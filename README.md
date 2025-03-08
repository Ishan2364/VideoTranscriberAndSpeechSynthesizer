# YouTube Video Downloader, Transcriber, and Text-to-Speech Converter

This script downloads a YouTube video, extracts its audio, transcribes it using Deepgram's API, and generates speech output using gTTS.

## Features
- Downloads YouTube videos.
- Extracts audio from the downloaded video.
- Transcribes audio using Deepgram's API.
- Converts the transcription into speech using gTTS.
- Automatically removes old audio files before downloading new ones.

## Requirements
Ensure you have the required dependencies installed:

```bash
pip install yt-dlp requests gtts
```

## Usage
1. Set up your Deepgram API credentials:
   - Replace `DEEPGRAM_API_KEY` with your API key.
   - Update `DEEPGRAM_API_URL` with the correct endpoint.

2. Run the script in a Python environment:

```python
python script.py
```

3. The script will:
   - Download and extract audio from the YouTube video.
   - Transcribe the extracted audio.
   - Generate speech output from the transcription.

## Example Output
```
Download completed successfully.
Audio extraction completed successfully.
Transcription completed successfully:
"This is the transcript of the video."
Audio generated successfully and saved as 'generated_audio.mp3'.
```

## Notes
- Ensure `ffmpeg` is installed for audio extraction.
- The YouTube video URL must be accessible.
- The script may need adjustments based on Deepgram API updates.

## License
This project is licensed under the MIT License.

