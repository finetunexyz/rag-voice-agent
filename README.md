# 🎤 🎙️ Voice-Based RAG App - Talk to Your Documents

A voice-enabled Retrieval-Augmented Generation (RAG) application built with **OpenAI's SDK** and **Streamlit**.  
It lets you upload PDF documents, ask questions, and receive both **text** and **voice** answers using OpenAI’s **Text-to-Speech (TTS)**.

---

## 🚀 Features
- **Voice-Enabled RAG System** using OpenAI SDK  
- **PDF Upload & Processing** with document chunking  
- **Qdrant Vector Database** for efficient similarity search  
- **Multiple Voice Options** for AI-generated speech  
- **Audio Download** capability (MP3)  
- **Multiple Document Support** with source tracking  
- **Real-Time Audio Streaming** via Streamlit  

---

## 🛠 How It Works

### 1️⃣ Document Processing
- Upload PDFs in the Streamlit interface  
- Split into chunks with LangChain’s `RecursiveCharacterTextSplitter`  
- Embed chunks with **FastEmbed** and store in **Qdrant**  

### 2️⃣ Query Processing
- Convert user question into embeddings  
- Retrieve relevant document chunks from Qdrant  
- Generate a **spoken-friendly answer** using an LLM  
- Pass the text through a **speech-optimized TTS agent**  

### 3️⃣ Voice Generation
- Convert response to speech via OpenAI TTS  
- Choose from **multiple voices**  
- Play audio in-browser or download as MP3  

---

## 📚 Tech Stack
- **OpenAI API** – Embeddings, LLM, and TTS  
- **LangChain** – Text splitting & RAG pipeline  
- **Qdrant** – Vector database for similarity search  
- **Streamlit** – Web interface  
- **FastEmbed** – High-speed embeddings  
