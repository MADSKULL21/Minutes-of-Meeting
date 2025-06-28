# Speech to Text Recorder

A simple desktop application to record your speech, convert it to text, and export the results to Word or PDF files. Built with Python, Tkinter, and Selenium for browser-based speech recognition.

## Features
- Start, pause, and stop speech recording
- Real-time transcription display
- Export transcribed text to Word (.docx) or PDF (.pdf)
- Simple, modern GUI

## How it Works
- Uses Selenium to launch a browser and leverage the browser's built-in speech recognition (Web Speech API)
- Captures recognized text and displays it in the GUI
- Allows exporting the text to Word or PDF with timestamps

## Setup Instructions

1. **Install Python 3.8+**
2. **Install Google Chrome** (required for Selenium WebDriver)
3. **Install dependencies:**
   ```bash
   pip install -r Requirements.txt
   ```
4. **Create a `.env` file** in the project root (optional, for language selection):
   ```
   InputLanguage = "en"
   ```
   - Default is English. You can use other language codes (e.g., "hi" for Hindi).

5. **Run the application:**
   ```bash
   python SpeechToTextGUI.py
   ```

## Usage
- Click **Start Recording** to begin.
- Speak into your microphone. The recognized text will appear in the window.
- Use **Pause** to temporarily stop, and **Stop** to finish.
- Export your text using the provided buttons.

## Requirements
- Python 3.8 or higher
- Google Chrome browser
- Microphone
- Internet connection (for Web Speech API)

## Project Structure
- `SpeechToTextGUI.py` — Main GUI application
- `SpeechToText.py` — Handles browser-based speech recognition
- `Data/` — Stores temporary HTML for recognition
- `.env` — (Optional) Language configuration

## Notes
- The application uses the browser's speech recognition, which may require microphone permissions.
- For best results, speak clearly and in a quiet environment.
- If you encounter issues with Selenium or ChromeDriver, ensure Chrome is installed and up to date.
