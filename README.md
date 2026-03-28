# Audio Mashup Web Service

A simple, locally-hosted web application built with Flask that allows you to create custom audio mashups of your favorite singers directly from YouTube.

## 🌟 Features
* **Simple Web Interface:** Easy-to-use HTML form to input your preferences.
* **Automated Downloading:** Uses `yt-dlp` to search and download the best quality audio for a specified artist.
* **Audio Processing:** Uses `pydub` to slice the first *Y* seconds of each downloaded video and merge them into a single audio file.
* **Direct Download:** Automatically packages the final `.mp3` mashup into a `.zip` file and prompts a download right in your browser.

## 📋 Prerequisites

Before running this application, you must have the following installed on your machine:
1. **Python 3.x**
2. **FFmpeg:** This is a crucial system dependency required by the `pydub` library to process and merge audio files. 

### How to Install FFmpeg:
* **Windows:** Download the pre-compiled binaries from the official site, extract them, and add the `bin` folder to your system's Environment Variables (PATH).
* **macOS:** Open terminal and run `brew install ffmpeg` (requires Homebrew).
* **Linux (Debian/Ubuntu):** Open terminal and run `sudo apt update && sudo apt install ffmpeg`.

## ⚙️ Installation & Setup

1. **Clone or Download** this repository to your local machine.
2. **Open a terminal** or command prompt and navigate to the project folder.
3. **Install the required Python libraries** by running:
   ```bash
   pip install flask yt-dlp pydub
