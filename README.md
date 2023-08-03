# OpenAI-Meeting-Minutes
An automated meeting minutes generator with Whisper and GPT-4.

## Based on this tutorial:
https://platform.openai.com/docs/tutorials/meeting-minutes

## Usage
Works out-of-the-box if you've pip installed `openai` and `python-docx`. However, you must supply an OpenAI API key at the top of the file.

## Caveats
 - API usage will cost some money, about $1-2/hr of audio
 - The Whisper API has a hard limit of 25 MB per audio file

## Tips
 - Shrink the size of your audio files: I use GarageBand to export them as Low Quality (64 kBit/s) MP3 files
 - If you can't get your audio file under 25 MB, you'll have to split it up into chunks, transcribe each chunk separately, then concatenate the transcription strings together to obtain the minutes (this would require tweaking the code)
