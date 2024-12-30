![SfondoPolitoSbobinatore](https://github.com/user-attachments/assets/5de48403-df52-4129-aa76-13939ba5d6f0)

# PolitoSbobinatore & UniversalSbobinatore 📚

🎓 Are you tired of struggling with messy lecture notes and spending endless hours transcribing recorded lessons? 😫 Say goodbye to those late nights trying to decipher your handwriting or watching hours of video lectures. 

✨ PolitoSbobinatore is here to revolutionize your study routine! 🚀

Your AI-powered note-taking assistant will handle everything automatically 🤖 - from downloading lecture videos to creating perfect transcriptions and concise summaries. While you focus on understanding concepts 🧠, our advanced AI technology works behind the scenes, transforming lengthy lectures into clear, well-structured study materials. 📚

Stop wasting time on manual transcription and start learning more effectively! 💪 With just one click, PolitoSbobinatore turns your video lectures into comprehensive notes that you can review anytime, anywhere. Transform your academic journey from exhausting to effortless. ⚡️

The future of note-taking is here. Let PolitoSbobinatore be your secret weapon for academic success! 🎯 

*Note: Please use responsibly and in accordance with PoliTo's academic policies.* ⚠️

A Python-based tool that automatically downloads, transcribes, and summarizes Politecnico di Torino virtual classroom lectures. This tool helps students create study notes from recorded lectures using AI-powered transcription and summarization.

# Not from Polito? Don't Worry! 🎓✨  

For you, there's **UniversalSbobinatore**! 🚀  
Simply upload the video of your lecture, and let it do the work for you. 🖥️📚  

No more stress—just smarter learning! 💡✅

# 📋 PolitoSbobinatore Feedback Form 🚀✨  

Thank you for helping us improve PolitoSbobinatore! 🌟 Your feedback is invaluable in making this tool more effective and user-friendly. Please take a few minutes to evaluate its features and share your thoughts.  

👉 Click the button below to fill out the form:  

[![📝 Fill the Feedback Form](https://img.shields.io/badge/📝_Fill_the_Form-Feedback-blueviolet?style=for-the-badge&logo=googleforms)](https://forms.gle/Caqherexh8jfQxrK6)  

Your insights will help us make PolitoSbobinatore even better! 💡  
Thank you for your time! 🙌  

# Support the Project 💖

If you find this project helpful, consider supporting me:

  <a href='https://ko-fi.com/martons00' target="_blank" rel="noopener noreferrer"><img height='42' style='border:0px;height:42px;' src='https://cdn.ko-fi.com/cdn/kofi3.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 
 [![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.me/RaffaeleMartone00)


[![satispayLogo](https://github.com/user-attachments/assets/47c1a538-7b9a-4cee-9b34-6ec1591136f9)](https://web.satispay.com/download/qrcode/S6Y-CON--471B0FCD-7946-4D72-A3BA-ACE837FF9D4F?)


# Table of Contents
- [PolitoSbobinatore \& UniversalSbobinatore 📚](#politosbobinatore--universalsbobinatore-)
- [Not from Polito? Don't Worry! 🎓✨](#not-from-polito-dont-worry-)
- [📋 PolitoSbobinatore Feedback Form 🚀✨](#-politosbobinatore-feedback-form-)
- [Support the Project 💖](#support-the-project-)
- [Table of Contents](#table-of-contents)
- [Features](#features)
- [Usage 🚀](#usage-)
  - [1. Local Installation 💻](#1-local-installation-)
  - [2. Google Colab PolitoSbobinatore (Recommended) ☁️](#2-google-colab-politosbobinatore-recommended-️)
    - [New to Google Colab? Here's a quick guide for PolitoSbobinatore:](#new-to-google-colab-heres-a-quick-guide-for-politosbobinatore)
        - [Video Tutorial](#video-tutorial)
  - [⚠️ **Important Note**: Free Google Colab has daily usage limits. Use your computation time wisely and consider upgrading to Colab Pro for extended usage.](#️-important-note-free-google-colab-has-daily-usage-limits-use-your-computation-time-wisely-and-consider-upgrading-to-colab-pro-for-extended-usage)
  - [3. Google Colab UniversalSbobinatore (Recommended) ☁️](#3-google-colab-universalsbobinatore-recommended-️)
    - [New to Google Colab? Here's a quick guide for UniversalSbobinatore:](#new-to-google-colab-heres-a-quick-guide-for-universalsbobinatore)
- [Output Files](#output-files)
- [Prerequisites](#prerequisites)
  - [**System Tools**](#system-tools)
  - [**Python Packages**](#python-packages)
- [Technical Details](#technical-details)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)

# Features

- 🔐 Automatic login to PoliTo platform
- 📥 Downloads lecture videos from Virtual Classroom
- 🎵 Extracts audio from video files
- 📝 Transcribes lectures using OpenAI's Whisper model
- ✍️ Generates summarized notes using BART large model
- 🤖 Handles long lectures by processing them in chunks
  
![Frame 237818](https://github.com/user-attachments/assets/3dc076b7-10fa-47e7-8eda-0d93c08e2f2a)
    
# Usage 🚀

There are two ways to use PolitoSbobinatore:

## 1. Local Installation 💻

If you have a powerful machine, you can run it locally. Note that you might need to adjust the web scraping component based on your system configuration and dependancies.

## 2. Google Colab PolitoSbobinatore (Recommended) ☁️

The easiest way to get started is using Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17qaSuauYw_Ms_iZVlPC0lvlCHsBjQ0DC?usp=sharing)

*Video Tutorial Below*

### New to Google Colab? Here's a quick guide for PolitoSbobinatore:


#### Video Tutorial  
[![Watch the video tutorial](https://img.youtube.com/vi/K8NnhIwUqvk/maxresdefault.jpg)](https://youtu.be/K8NnhIwUqvk)  



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

😇 **Rest assured, your data will be available exclusively to you and only on your Drive.** 😇

<img width="895" alt="Screenshot 2024-12-05 at 01 32 45" src="https://github.com/user-attachments/assets/7041c1ae-08b5-45df-951d-a2fb68df0c11">


## 3. Google Colab UniversalSbobinatore (Recommended) ☁️

The easiest way to get started is using Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1oApOVY0ccpVDnNGTRf55dOmdMscNsRs0?usp=sharing)

### New to Google Colab? Here's a quick guide for UniversalSbobinatore:

Before running the notebook:
1. Upload your video, dragging and drop in the area in the screenshot
2. Fill the variable with the name of your video 
3. Run all cells in sequence
4. 
<img width="632" alt="Screenshot 2024-12-17 at 14 44 51" src="https://github.com/user-attachments/assets/54ba4a2d-9a34-4558-88c5-c462f959ef27" />


⚠️ **Tips**: Download the transcription.txt and summary.txt and use it in a more complex LLM to a better results. Free Models have some limitations.

The tool will handle the rest automatically! 🎯

# Output Files

- `video.mp4`: Downloaded lecture video
- `audio.mp3`: Extracted audio from the video
- `trascrizione.txt`: Full transcription of the lecture
- `final_summary.txt`: Summarized version of the lecture


# Prerequisites
The following packages and tools need to be installed:
## **System Tools**  
- Python 3.x  
- ffmpeg  
- Chromium Browser  
- ChromeDriver  

## **Python Packages**  
- whisper  
- moviepy  
- transformers  
- torch  
- selenium  
- webdriver_manager  
- requests  


# Technical Details

- Uses Selenium WebDriver for web automation
- Implements OpenAI's Whisper model for transcription
- Utilizes Facebook's BART-large-cnn model for summarization
- Processes long lectures in chunks of 1024 characters
- Handles browser automation in headless mode

# Limitations

- Requires stable internet connection
- Processing time depends on lecture length
- Summary quality may vary based on audio quality
- Limited to PoliTo virtual classroom platform
- Computational expensive, it can take time
- Bart-Large-CNN will be not very precise or exhausting 

# Contributing

Feel free to submit issues and pull requests to help improve this tool.

# Disclaimer

This tool is for educational purposes only. Make sure to comply with Politecnico di Torino's policies regarding lecture recordings and content usage.

# License

MIT License

Copyright (c) 2024 Raffaele Martone

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
