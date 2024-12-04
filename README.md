# PolitoSbobinatore 📚

A Python-based tool that automatically downloads, transcribes, and summarizes Politecnico di Torino virtual classroom lectures. This tool helps students create study notes from recorded lectures using AI-powered transcription and summarization.

## Features

- 🔐 Automatic login to PoliTo platform
- 📥 Downloads lecture videos from Virtual Classroom
- 🎵 Extracts audio from video files
- 📝 Transcribes lectures using OpenAI's Whisper model
- ✍️ Generates summarized notes using BART large model
- 🤖 Handles long lectures by processing them in chunks

## Prerequisites

The following packages and tools need to be installed:

- Python 3.x
- ffmpeg
- ChromeDriver
- Required Python packages:
  - openai-whisper
  - moviepy
  - transformers
  - torch
  - selenium
  - requests

flowchart TD
    A[Start] --> B[Web Scraping]
    subgraph Web Scraping
        B -->|Selenium| C[Login to PoliTo]
        C --> D[Navigate to Course]
        D --> E[Download Video]
    end
    
    subgraph Video Processing
        E -->|MoviePy| F[Extract Audio]
        F -->|.mp4 to .mp3| G[Audio File]
    end
    
    subgraph Transcription
        G -->|Whisper AI| H[Raw Transcription]
        H -->|Save| I[trascrizione.txt]
    end
    
    subgraph Summarization
        I -->|BART Model| J[Process text chunks]
        J -->|Generate Summary| K[final_summary.txt]
    end
    
    K --> L[End]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style L fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style F fill:#bfb,stroke:#333,stroke-width:2px
    style H fill:#fbf,stroke:#333,stroke-width:2px
    style J fill:#fbb,stroke:#333,stroke-width:2px
    
## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/politosbobinatore.git
cd politosbobinatore
```

2. Install the required packages:
```bash
pip install git+https://github.com/openai/whisper.git
pip install moviepy transformers torch selenium requests
```

3. Install system dependencies:
```bash
sudo apt update
sudo apt install ffmpeg chromium-browser chromedriver
```

## Configuration

Before running the script, you need to set up your credentials and course information:

```python
USERNAME = "your_polito_username"
PASSWORD = "your_polito_password"
COURSE_TITLE = "your_course_name"
LECTURE_TITLE = "specific_lecture_name"
```

## Usage

1. Set up your credentials and course information in the script
2. Run the script:
```bash
python politosbobinatore.py
```

The script will:
1. Log in to your PoliTo account
2. Navigate to the specified course and lecture
3. Download the lecture video
4. Convert the video to audio
5. Transcribe the audio using Whisper
6. Generate a summarized version using BART
7. Save both the transcription and summary as text files

## Output Files

- `video.mp4`: Downloaded lecture video
- `audio.mp3`: Extracted audio from the video
- `trascrizione.txt`: Full transcription of the lecture
- `final_summary.txt`: Summarized version of the lecture

## Technical Details

- Uses Selenium WebDriver for web automation
- Implements OpenAI's Whisper model for transcription
- Utilizes Facebook's BART-large-cnn model for summarization
- Processes long lectures in chunks of 1024 characters
- Handles browser automation in headless mode

## Limitations

- Requires stable internet connection
- Processing time depends on lecture length
- Summary quality may vary based on audio quality
- Limited to PoliTo virtual classroom platform

## Contributing

Feel free to submit issues and pull requests to help improve this tool.

## Disclaimer

This tool is for educational purposes only. Make sure to comply with Politecnico di Torino's policies regarding lecture recordings and content usage.

## License

[Add your chosen license here]
