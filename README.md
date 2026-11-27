# YouTubeIQ – Intelligent Video Knowledge Assistant

An AI-powered YouTube video knowledge assistant that uses **Google Gemini**, **LangChain**, and **Retrieval-Augmented Generation (RAG)** to understand YouTube video transcripts and answer user questions with context-aware responses.

## 🚀 Overview

YouTubeIQ allows users to ask questions about YouTube videos and receive answers based on the video's transcript.

The application follows a RAG pipeline to retrieve relevant information from video transcripts and generate meaningful responses using Google's Gemini LLM.

## ✨ Features

- YouTube video transcript processing
- Text splitting and chunking
- Semantic embeddings
- Vector similarity search using FAISS
- Context-aware question answering
- Google Gemini integration
- Retrieval-Augmented Generation (RAG)

## 🛠️ Tech Stack

- **Programming Language:** Python
- **LLM:** Google Gemini
- **Framework:** LangChain
- **Vector Database:** FAISS
- **Embeddings:** Hugging Face / configured embedding model
- **Environment Management:** Python dotenv
- **Development Environment:** Jupyter Notebook

## 📁 Project Structure

```text
YouTubeIQ/
├── ragf.ipynb
├── transcript.txt
├── .env.example
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Shree0106/YouTubeIQ.git
cd YouTubeIQ
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

Linux/macOS:
```bash
source .venv/bin/activate
```

### 3. Install dependencies

Install the packages required by the notebook.

```bash
pip install langchain langchain-community langchain-google-genai faiss-cpu python-dotenv
```

Install any additional packages imported in the notebook.

### 4. Configure API Key

Create a `.env` file using `.env.example` as a template.

Add your Google Gemini API key:

```env
GOOGLE_API_KEY=your_api_key_here
```

Never upload your actual API key to GitHub.

### 5. Run the application

Open the Jupyter Notebook:

```bash
jupyter notebook ragf.ipynb
```

Execute the notebook cells in sequence.

## 🧠 How It Works

1. Extract or load the YouTube video transcript.
2. Split the transcript into smaller text chunks.
3. Generate embeddings for the text chunks.
4. Store embeddings in FAISS.
5. Convert the user's question into an embedding.
6. Retrieve the most relevant transcript chunks.
7. Pass the retrieved context and question to Google Gemini.
8. Generate a context-aware answer.

## 🎯 Learning Outcomes

- Understanding Retrieval-Augmented Generation (RAG).
- Working with Large Language Models.
- Implementing semantic search and embeddings.
- Understanding vector databases.
- Integrating Google Gemini with LangChain.
- Building practical Generative AI applications.

## 👨‍💻 Author

**Shrinivas Pampatwar**

GitHub: https://github.com/Shree0106