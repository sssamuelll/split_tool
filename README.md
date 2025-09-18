# Audio Splitter Tool

A simple Python tool to split an audio file into smaller chunks of a specified duration and save them as MP3 files.

## Features
- Split any audio file into smaller chunks.
- Default chunk duration: **30 minutes**.
- Save output as MP3 files in a dedicated folder.
- Customizable chunk duration.

## Requirements
- Python 3.x
- [pydub](https://github.com/jiaaro/pydub)  
  Install with:
  pip install -r requirements.txt
- [ffmpeg](https://ffmpeg.org/)  
  Make sure it is installed and available in your system PATH.

## Installation
Clone this repository and navigate into the folder:

git clone https://github.com/yourusername/audio-splitter.git
cd audio-splitter

Make the script executable:
chmod +x split_tool

## Usage
Run the script directly from the command line:

./split_tool <audio_file> [--chunk_duration MINUTES]

### Examples
Split an audio file into 30-minute chunks (default):
./split_tool audio.wav

Split an audio file into 15-minute chunks:
./split_tool audio.wav --chunk_duration 15

### Output
The chunks will be saved in a folder named:
<filename>_chunks/

Each file will be named:
chunk_1.mp3, chunk_2.mp3, ...

## Notes
- Works with any audio format supported by **ffmpeg**.
- Large files may take longer to process.

## License
MIT License
