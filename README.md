# Real-Time Voice AI Agent with LiveKit

This project is a real-time voice AI assistant built using [LiveKit Agents](https://docs.livekit.io/agents/). It leverages advanced speech-to-text (STT), large language models (LLM), and text-to-speech (TTS) technologies to enable interactive voice conversations. The agent can join LiveKit rooms, process audio, and respond intelligently.

## Project Overview

* **LiveKit Agents:** Orchestrates real-time audio, STT, LLM, and TTS.
* **Deepgram:** Speech-to-text (STT) plugin.
* **Cartesia:** Text-to-speech (TTS) plugin.
* **Silero:** Voice activity detection (VAD).
* **Noise Cancellation:** Pre-built plugin for audio enhancement.
* **Turn Detector:** Multimodal LLM for detecting speaker turns.
* **OpenAI/Groq:** Large language model (LLM) integration.
* **Python:** Main programming language.
* **python-dotenv:** For environment variable management.

## Setup Instructions

### 1. Clone the Repository

Clone the project to your local machine and navigate into the directory.

```bash
git clone git@github.com:affafghani98/-Real-Time-Voice-AI-Agent.git
cd -Real-Time-Voice-AI-Agent
```
### 2. Create and Activate Virtual Environment

It is recommended to use a virtual environment to manage project dependencies.

On Windows:

```bash
python -m venv venv
.\venv\Scripts\activate
```



### 3. Install Dependencies

Install all the necessary packages using pip.

```bash
pip install "livekit-agents[deepgram,cartesia,silero,turn-detector]~=1.2" \
            "livekit-plugins-noise-cancellation~=0.2" \
            "livekit-plugins-openai~=1.2" \
            "python-dotenv"
pip install livekit-plugins-openai

```

### 4.Set Up Environment Variables

Create a .env file in the project's root directory and add your API keys and credentials.
```bash
LIVEKIT_URL=your_livekit_url
LIVEKIT_API_KEY=your_livekit_api_key
LIVEKIT_API_SECRET=your_livekit_api_secret
GROQ_API_KEY=your_groq_api_key
DEEPGRAM_API_KEY=your_deepgram_api_key
CARTESIA_API_KEY=your_cartesia_api_key
```

### 5. Run the Agent

Once everything is set up, you can run the agent from your terminal.
```bash
python agent.py console
```
