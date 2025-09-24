# Jarvis Voice Assistant 🤖

A Python-based voice assistant named "Jarvis" that can perform various tasks through voice commands. The assistant responds to a wake word and can open websites, play music, search for information, and more.

## Features ✨

- **Voice Recognition**: Uses Google's speech recognition API
- **Text-to-Speech**: Converts responses to audio using Google TTS
- **Wake Word Activation**: Responds to "Jarvis" as wake word
- **Web Automation**: Opens various websites (Instagram, YouTube, GitHub, LinkedIn, etc.)
- **Music Player**: Plays songs from a custom library via YouTube links
- **Information Search**: Wikipedia integration for quick facts
- **Google Search**: Voice-activated web searching
- **Multilingual Support**: Supports both Hindi and English commands

## Project Structure 📁

```
Jarvis-Voice-Assistant/
├── Jarvis.py           # Main voice assistant script
├── music_library.py    # Music database with YouTube links
├── requirements.txt    # Python dependencies
└── README.md          # Project documentation
```

## Installation & Setup 🚀

### Prerequisites
- Python 3.7 or higher
- Microphone for voice input
- Internet connection for TTS and web features

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/Jarvis-Voice-Assistant.git
cd Jarvis-Voice-Assistant
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

**Note**: If you encounter issues with PyAudio installation:

**Windows:**
```bash
pip install pipwin
pipwin install pyaudio
```

**macOS:**
```bash
brew install portaudio
pip install pyaudio
```

**Linux (Ubuntu/Debian):**
```bash
sudo apt-get install python3-pyaudio
```

## Usage 💬

### Running the Assistant
```bash
python Jarvis.py
```

### Voice Commands

**Wake Word**: Say "Jarvis" to activate the assistant

**Supported Commands**:
- **"open instagram"** or **"instagram khol"** - Opens Instagram
- **"open youtube"** or **"youtube khol"** - Opens YouTube  
- **"open github"** or **"coders ka adda"** - Opens GitHub
- **"open linkedin"** or **"demotivate kar"** - Opens LinkedIn
- **"model"** or **"moodle"** - Opens IIT Patna Moodle
- **"meri playlist chala"** - Plays your custom playlist
- **"google [topic]"** or **"search [topic]"** - Google search
- **"play [song name]"** - Plays song from music library
- **"information about [topic]"** - Wikipedia search
- **"tell me about [topic]"** - Wikipedia search
- **"who is [person]"** - Wikipedia search
- **"tum best ho"** - Compliment the assistant
- **"good bye"** - Say goodbye
- **"exit"** or **"quit"** - Shut down the assistant

### Music Library
The assistant includes a curated music library with popular Hindi songs:
- Awarapan
- Hale Dil
- Woh Lamhe
- Zara Sa
- Tu Hi Mera
- Shera
- Najar Ka Teer
- Bulleya
- Safari
- Haseen

## Customization 🎨

### Adding New Songs
Edit `music_library.py` to add more songs:
```python
music = {
    "song_name": "youtube_link",
    "new_song": "https://youtu.be/your_link_here"
}
```

### Adding New Commands
Modify the `myCommand(c)` function in `Jarvis.py` to add custom voice commands.

### Changing Voice Settings
Adjust the TTS settings in the `speak()` function:
```python
tts = gTTS(text=text, lang="en", slow=False)  # Change lang to "hi" for Hindi
```

## Troubleshooting 🔧

### Common Issues:

1. **Microphone not working**: Check microphone permissions and ensure it's properly connected
2. **PyAudio installation errors**: Follow the OS-specific installation instructions above
3. **Internet connectivity**: Ensure stable internet for TTS and web features
4. **Wake word not recognized**: Speak clearly and ensure minimal background noise

### Error Handling
The assistant includes error handling for:
- Speech recognition failures
- Network connectivity issues
- Missing audio files
- Wikipedia search errors

## Requirements 📋

- speechrecognition==3.10.0
- gTTS==2.3.2
- playsound==1.3.0
- wikipedia==1.4.0
- PyAudio==0.2.11

## Contributing 🤝

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## License 📄

This project is open source and available under the [MIT License](LICENSE).

## Author 👨‍💻

Created by [Your Name] - feel free to contact me for any questions or suggestions!

## Acknowledgments 🙏

- Google Speech Recognition API
- Google Text-to-Speech API
- Wikipedia API
- Python community for amazing libraries

---

**Enjoy using Jarvis Voice Assistant! 🚀**

## 👨‍💻 Developer

**ASMIT SRIVASTAVA** 

💼 **LinkedIn:** [Connect with me](https://www.linkedin.com/in/asmit-srivastava-178420315/)  
📸 **Instagram:** [@hey.asmit](https://www.instagram.com/hey.asmit/)  
