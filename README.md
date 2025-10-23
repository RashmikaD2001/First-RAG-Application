# 🧠 Retrieval-Augmented Generation (RAG) using LangChain + Google Gemini

This project demonstrates a simple **Retrieval-Augmented Generation (RAG)** pipeline built with **LangChain**, **Chroma**, and **Google Gemini**.

It loads Markdown (`.md`) documents, splits them into smaller chunks, stores them in a **Chroma vector database**, and uses **Gemini** to generate intelligent, context-based answers to user queries.

---

## 🚀 Features

- 🗂️ Load and process Markdown documents from a local `data/` directory  
- 🧩 Split text into manageable overlapping chunks  
- 🧠 Generate embeddings using **Google Generative AI (Gemini Embeddings)**  
- 💾 Store and retrieve document vectors using **Chroma**  
- 💬 Generate answers with **Gemini 2.0 Flash** using retrieved context  
- ⚙️ Fully script-based workflow (no need for a web app or UI)

---

## 📁 Project Structure
```
├── data/ # Markdown files for embedding
├── chroma/ # Persisted Chroma vector database
├── .env # Contains GOOGLE_API_KEY
├── main.py # Document loader, splitter, and DB builder
└── query.py # Query interface using Gemini + Chroma
```

---

## 🔑 Requirements

- Python 3.10+
- [Google API key](https://aistudio.google.com/app/apikey)
