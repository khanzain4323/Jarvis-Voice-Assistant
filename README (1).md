# Jarvis Voice Assistant 🎙️

A simple Python-based voice assistant (inspired by Alexa/Google Assistant) that listens for a wake word, understands voice commands, and can open websites, play music, or answer general questions using OpenAI's GPT model.

## Features

- 🎧 Wake-word activated ("Jarvis")
- 🌐 Opens popular websites (YouTube, Google, Facebook, Twitter, Instagram) via voice
- 🎵 Plays songs from a personal music library
- 🤖 Answers general questions using OpenAI's GPT-3.5 model
- 🔊 Speaks responses back using text-to-speech

## Tech Stack

- Python
- [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) — converts speech to text
- [pyttsx3](https://pypi.org/project/pyttsx3/) — text-to-speech engine
- [OpenAI Python SDK](https://pypi.org/project/openai/) — GPT-3.5 responses

## Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/jarvis-voice-assistant.git
cd jarvis-voice-assistant
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Add your OpenAI API key
Create a `.env` file in the root folder (this file is ignored by Git and never uploaded):
```
OPENAI_API_KEY=your_actual_key_here
```

> ⚠️ Never hardcode your API key directly in `.py` files. Always use environment variables.

### 4. Run the assistant
```bash
python main.py
```

Say **"Jarvis"** to activate, then speak your command — e.g. "open YouTube", "play At peace", or ask it any question.

## Project Structure

```
jarvis-voice-assistant/
├── main.py
├── musicLibrary.py
├── client.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## Security Note

This project reads the API key from an environment variable, not from source code. Never commit real API keys to GitHub — if one is ever exposed, revoke it immediately from your provider's dashboard.

## License

This project is open source and available under the [MIT License](LICENSE).
