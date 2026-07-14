# 📄 DocMind AI

> **An AI-powered PDF Learning Assistant built with Streamlit, LangChain, FAISS, HuggingFace Embeddings, and Groq Llama 3.3.**

DocMind AI transforms any PDF into an interactive learning experience. Upload your notes, textbooks, research papers, or documentation and instantly chat with them, generate AI summaries, create flashcards, take quizzes, and export your study notes.

---

## 🚀 Features

### 💬 Chat with your PDF
- Ask natural language questions about any uploaded PDF.
- Powered by Retrieval-Augmented Generation (RAG).
- Context-aware answers using semantic search.

### 🧠 AI Summary
- Generates concise summaries of lengthy PDFs.
- Highlights key concepts and important information.

### 📚 Flashcard Generator
- Automatically creates study flashcards from the document.
- Interactive "Show Answer" functionality.

### 📝 Quiz Generator
- Generates multiple-choice quizzes.
- Automatically grades answers.
- Displays final score.

### 🎤 Voice Chat
- Ask questions using your microphone.
- Speech-to-text powered by Groq Whisper.

### 📖 Export Notes
- Export:
  - AI Summary
  - Flashcards
  - Quiz
  - Chat History
- Downloads as a Microsoft Word (.docx) document.

### 📌 Source Citations
- Every answer displays the page(s) where the information was found.

### 💾 Chat History
- Conversation persists during the session.
- Clean chat interface with avatars.

### ⚡ Semantic Search
- Uses HuggingFace embeddings with FAISS vector database for fast and relevant document retrieval.

---

# 🏗️ Tech Stack

## Frontend
- Streamlit

## AI
- Groq API
- Llama 3.3 70B Versatile
- Whisper Large v3

## RAG Pipeline
- LangChain
- FAISS
- HuggingFace Embeddings

## Document Processing
- PyPDF2

## Export
- python-docx

---

# 🧠 Architecture

```
                PDF
                 │
                 ▼
          Extract Text
                 │
                 ▼
          Split into Chunks
                 │
                 ▼
     HuggingFace Embeddings
                 │
                 ▼
          FAISS Vector DB
                 │
                 ▼
     Similarity Search (RAG)
                 │
                 ▼
      Relevant Context Chunks
                 │
                 ▼
      Groq Llama 3.3 70B
                 │
                 ▼
           AI Response
```

---

# 📂 Project Structure

```
DocMind-AI/
│
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
├── README.md
│
└── assets/
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/Lilakhiz/DocMind-AI.git
```

Go into the project

```bash
cd DocMind-AI
```

Install dependencies

```bash
pip install -r requirements.txt
```

Create a `.env`

```env
GROQ_API_KEY=your_api_key
```

Run the app

```bash
streamlit run app.py
```

---

# 🎯 How it Works

1. Upload a PDF.
2. Text is extracted using PyPDF2.
3. The document is split into manageable chunks.
4. HuggingFace Embeddings convert text into vectors.
5. FAISS indexes those vectors.
6. User questions are converted into embeddings.
7. Similar chunks are retrieved using semantic search.
8. Retrieved context is sent to Groq Llama 3.3.
9. AI generates an answer grounded in the uploaded document.

---

# 📸 Features Preview

### 📄 PDF Chat
- Ask questions naturally.
- Context-aware responses.
- Page citations.

### 🧠 AI Summary
Generate concise study notes in one click.

### 📚 Flashcards
Automatically generate revision flashcards.

### 📝 Quiz Generator
Practice using AI-generated MCQs.

### 🎤 Voice Chat
Talk to your PDF using speech recognition.

### 📖 Export Notes
Download all generated notes as a Word document.

---

# 🔥 Future Improvements

- Multiple PDF support
- Conversation memory across sessions
- PDF highlighting of cited passages
- OCR support for scanned PDFs
- Dark/Light theme toggle
- User authentication
- Cloud storage integration
- Study progress dashboard

---

# 🛠️ Built With

- Streamlit
- LangChain
- FAISS
- HuggingFace Embeddings
- Groq API
- Whisper Large v3
- PyPDF2
- python-docx

---

# 👨‍💻 Developed By

**Akhilesh**

### Connect with me

- 💼 LinkedIn: https://www.linkedin.com/in/YOUR-LINKEDIN
- 🐙 GitHub: https://github.com/Lilakhiz

---

## ⭐ If you found this project useful, consider giving it a star!
