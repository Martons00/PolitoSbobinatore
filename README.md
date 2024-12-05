# PolitoSbobinatore 📚

🎓 Are you tired of struggling with messy lecture notes and spending endless hours transcribing recorded lessons? 😫 Say goodbye to those late nights trying to decipher your handwriting or watching hours of video lectures. 

✨ PolitoSbobinatore is here to revolutionize your study routine! 🚀

Your AI-powered note-taking assistant will handle everything automatically 🤖 - from downloading lecture videos to creating perfect transcriptions and concise summaries. While you focus on understanding concepts 🧠, our advanced AI technology works behind the scenes, transforming lengthy lectures into clear, well-structured study materials. 📚

Stop wasting time on manual transcription and start learning more effectively! 💪 With just one click, PolitoSbobinatore turns your video lectures into comprehensive notes that you can review anytime, anywhere. Transform your academic journey from exhausting to effortless. ⚡️

The future of note-taking is here. Let PolitoSbobinatore be your secret weapon for academic success! 🎯 

*Note: Please use responsibly and in accordance with PoliTo's academic policies.* ⚠️

A Python-based tool that automatically downloads, transcribes, and summarizes Politecnico di Torino virtual classroom lectures. This tool helps students create study notes from recorded lectures using AI-powered transcription and summarization.

## Features

- 🔐 Automatic login to PoliTo platform
- 📥 Downloads lecture videos from Virtual Classroom
- 🎵 Extracts audio from video files
- 📝 Transcribes lectures using OpenAI's Whisper model
- ✍️ Generates summarized notes using BART large model
- 🤖 Handles long lectures by processing them in chunks
  
![Frame 237818](https://github.com/user-attachments/assets/3dc076b7-10fa-47e7-8eda-0d93c08e2f2a)
    
## Usage 🚀

There are two ways to use PolitoSbobinatore:

### 1. Local Installation 💻

If you have a powerful machine, you can run it locally. Note that you might need to adjust the web scraping component based on your system configuration.

### 2. Google Colab (Recommended) ☁️

The easiest way to get started is using Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17qaSuauYw_Ms_iZVlPC0lvlCHsBjQ0DC?usp=sharing)

#### New to Google Colab? Here's a quick guide:

1. Click the "Open in Colab" button above
2. Sign in with your Google account
3. Create a copy in your Drive by clicking `File → Save a copy in Drive`
   
   ![Save to Drive](https://github.com/user-attachments/assets/b78bab3e-e1df-4479-a83f-dcaf79f35337)

4. Select T4 GPU runtime for optimal performance:
   - Go to `Runtime → Change runtime type`
   - Select "T4 GPU" from the dropdown menu
   
   ![Change Runtime](https://github.com/user-attachments/assets/2ed00145-aad1-4d49-a7fb-a5502fffc0ac)

⚠️ **Important Note**: Free Google Colab has daily usage limits. Use your computation time wisely and consider upgrading to Colab Pro for extended usage.

---

Before running the notebook:
1. Fill in your PoliTo credentials
2. Enter your course and lecture details
3. Run all cells in sequence
<img width="895" alt="Screenshot 2024-12-05 at 01 32 45" src="https://github.com/user-attachments/assets/7041c1ae-08b5-45df-951d-a2fb68df0c11">

⚠️ **Tips**: Download the transcription.txt and summary.txt and use it in a more complex LLM to a better results. Free Models have some limitations.

The tool will handle the rest automatically! 🎯

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


## Prerequisites
The following packages and tools need to be installed:
### **System Tools**  
- Python 3.x  
- ffmpeg  
- Chromium Browser  
- ChromeDriver  

### **Python Packages**  
- whisper  
- moviepy  
- transformers  
- torch  
- selenium  
- webdriver_manager  
- requests  


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
