# MediSage - AI based Voice enabled Medical Chatbot

MediSage is a full-stack AI-powered RAG-assisted chatbot web application built using **Langchain**, **Flask**, **Pinecone API**, **Together API**, and **JavaScript Web Speech API**. It allows users to have a real-time chat experience where:

- Messages are sent to a Together AI-powered LLM
- The bot replies instantly in text and **voice**
- You can optionally upload audio files
- Uses `pydub` + `ffmpeg` for audio handling on the backend

---

## 🧠 Features

- 🔄 Real-time chat interface
- 🧑‍💻 Backend powered by **Together AI API**
- 🔊 Text-to-speech using **Web Speech API**
- 📁 Audio upload functionality
- 📜 Clean, animated UI with proper styling

---

## 🏗️ Tech Stack

| Layer        | Technology                              |
|--------------|-----------------------------------------|
| Frontend     | HTML, CSS, JavaScript                   |
| Backend      | Flask (Python)                          |
| AI Model     | Together API, Mistral-7B-Instruct (LLM) |
| Audio Output | Web Speech API + PyDub                  |
| Environment  | Conda (Python 3.9+)                     |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-voice-chatbot.git
cd ai-voice-chatbot
```

### 2. Create Conda Environment
```bash

conda create -n chatbot-env python=3.9
conda activate chatbot-env
```

### 3. Install Dependencies
```bash

pip install -r requirements.txt
```

Also install ffmpeg for pydub:

```bash

conda install -c conda-forge ffmpeg
```

### 4. Set Your Together API Key
### 5. Create a .env file and add:

TOGETHER_API_KEY=your_actual_key_here
Or set it in app.py directly if you're testing.

## 🏃 Run the App
```bash

python app.py
```

Visit http://localhost:5000 in your browser.

## 📁 **Project Structure**

├── app.py                 # Flask backend
├── templates/
│   └── chat.html          # Main chat UI
├── static/
│   ├── style.css          # Styling
│   └── scripts.js         # JS: Chat, TTS, file upload
├── requirements.txt       # Python deps
└── README.md              # You are here




## 💡**Future Enhancements:**

⏺️ Microphone input & live voice recognition

🧠 Add memory/context window to LLM

🗃️ Chat history and user login

📱 Mobile responsiveness

## 🙌 **Acknowledgements:**

Together AI

PyDub

MDN Web Speech API


