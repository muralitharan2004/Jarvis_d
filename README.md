# Jarvis_d
# Jarvis# 🎤 LiveKit Voice Assistant (Python)

This project is a **voice assistant powered by [LiveKit Agents](https://docs.livekit.io/agents/)** and **Google Gemini Realtime**.  
It captures user speech from a LiveKit room, processes it with a language model, and speaks back with synthesized voice — all in real time.

---

## ✨ What this project does
- Listens to microphone audio in a LiveKit room.
- Uses **Google Gemini Realtime** as the LLM for reasoning and response generation.
- Converts text responses into speech with a natural voice.
- Publishes assistant audio back into the same LiveKit room so participants hear it as if another user joined.
- Includes optional **LiveKit Cloud noise cancellation** for better audio quality.

---

## 🏗️ Project structure
/voice-assistant
├─ assistant.py # main entrypoint (this file)
├─ prompt.py # stores AGENT_INSTRUCTION and AGENT_RESPONSE text
├─ .env # environment variables (not committed to git)
└─ README.md # this file


---

## ⚙️ Requirements
- **Python 3.9+**
- [LiveKit Agents SDK](https://docs.livekit.io/agents/getting-started/python/)
- [Google Gemini Realtime](https://ai.google.dev/) credentials
- A [LiveKit Cloud](https://livekit.io/cloud) project (or self-hosted LiveKit server)

---

## 📦 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/yourusername/livekit-voice-assistant.git
cd livekit-voice-assistant
pip install -r requirements.txt



---

## ⚙️ Requirements
- **Python 3.9+**
- [LiveKit Agents SDK](https://docs.livekit.io/agents/getting-started/python/)
- [Google Gemini Realtime](https://ai.google.dev/) credentials
- A [LiveKit Cloud](https://livekit.io/cloud) project (or self-hosted LiveKit server)

---

## 📦 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/yourusername/livekit-voice-assistant.git
cd livekit-voice-assistant
pip install -r requirements.txt

python-dotenv
livekit-agents
livekit-plugins-google
livekit-plugins-noise-cancellation


# LiveKit API
LIVEKIT_URL=wss://your-livekit-server
LIVEKIT_API_KEY=your_api_key
LIVEKIT_API_SECRET=your_api_secret

# Google Gemini Realtime
GOOGLE_API_KEY=your_google_api_key


python assistant.py


AGENT_INSTRUCTION = """
You are a friendly voice assistant.
Answer clearly and concisely.
"""

AGENT_RESPONSE = """
Introduce yourself politely to new participants in the room.
"""

📖 Resources

LiveKit Agents Documentation

Google Gemini API

LiveKit Plugins

---

👉 Do you want me to also generate the `requirements.txt` file alongside this README so your GitHub repo is **ready to clone and run**?
