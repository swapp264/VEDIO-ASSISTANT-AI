# 🎥 AI Video Assistant

> **Transcribe • Summarize • Extract Insights • Chat with Your Meetings using AI**

AI Video Assistant is an end-to-end meeting intelligence platform that transforms YouTube videos, meeting recordings, and audio files into structured, searchable knowledge. It combines speech recognition, Retrieval-Augmented Generation (RAG), and Large Language Models to generate accurate meeting summaries, action items, decisions, and interactive Q&A.

---

## 🚀 Features

- 🎥 Accepts YouTube URLs
- 📁 Upload audio or video files
- 🎙️ English transcription using **OpenAI Whisper (Local)**
- 🇮🇳 Hindi & Hinglish transcription using **Sarvam AI**
- 📝 AI-generated meeting summaries
- ✅ Extracts Action Items with owners and deadlines
- 📌 Identifies Key Decisions
- ❓Extracts Open Questions & Follow-ups
- 💬 Chat with meeting transcripts using **RAG**
- 📄 Export reports as **PDF** or **TXT**
- ⚡ Modern Streamlit interface

---

## 🖥️ Demo

<img src="assets/demo.png" width="100%"/>

---

## 🏗️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| UI | Streamlit |
| Speech-to-Text | OpenAI Whisper |
| Hindi/Hinglish STT | Sarvam AI |
| LLM | Mistral AI |
| Framework | LangChain LCEL |
| Vector Database | ChromaDB |
| Embeddings | HuggingFace Sentence Transformers |
| RAG | LangChain + ChromaDB |
| PDF Export | ReportLab |
| Audio Processing | Pydub + FFmpeg |

---

## 📂 Project Structure

```
AI-Video-Assistant/
│
├── core/
│   ├── rag_engine.py
│   ├── vector_store.py
│   ├── summarizer.py
│   ├── extractor.py
│
├── utils/
│   ├── audio_processor.py
│   ├── transcription.py
│
├── app.py
├── main.py
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/AI-Video-Assistant.git

cd AI-Video-Assistant
```

### Create Virtual Environment

```bash
python -m venv .venv
```

Windows

```bash
.venv\Scripts\activate
```

Mac/Linux

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
MISTRAL_API_KEY=your_mistral_api_key
SARVAM_API_KEY=your_sarvam_api_key
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

The application will be available at:

```
http://localhost:8501
```

---

## 📋 Workflow

```text
YouTube URL / Audio / Video
            │
            ▼
     Audio Processing
            │
            ▼
 Speech-to-Text (Whisper / Sarvam)
            │
            ▼
      Transcript Generation
            │
            ▼
      AI Summarization
            │
            ├────────► Action Items
            │
            ├────────► Key Decisions
            │
            ├────────► Open Questions
            │
            ▼
      ChromaDB Vector Store
            │
            ▼
      RAG Question Answering
            │
            ▼
     Export PDF / TXT Report
```

---

## 💡 Example Use Cases

- Corporate Meeting Analysis
- Interview Summarization
- Lecture Notes Generation
- Podcast Summaries
- Webinar Analysis
- Customer Meeting Documentation
- Team Standups
- Project Review Meetings

---

## 🎯 Key Highlights

- Local Whisper transcription (No OpenAI API cost)
- Hindi & Hinglish support
- AI-generated meeting intelligence
- Retrieval-Augmented Generation (RAG)
- Interactive meeting chat
- Modern responsive UI
- PDF & TXT report export
- End-to-end automated workflow

---

## 📦 Future Improvements

- Multi-language translation
- Speaker diarization
- Real-time meeting transcription
- Meeting sentiment analysis
- Email report sharing
- Cloud deployment
- Calendar integration
- Team collaboration dashboard

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Swapnil Raskar**

---

⭐ If you found this project useful, don't forget to star the repository!