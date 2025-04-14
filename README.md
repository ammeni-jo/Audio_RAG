# Audio_RAG
# 🎧 Audio RAG with DeepSeek-R1

While most Retrieval-Augmented Generation (RAG) systems focus on text, **a vast amount of valuable data exists in the form of speech**. This project demonstrates how to build a RAG pipeline designed specifically for **audio files**, powered by **DeepSeek-R1** and **AssemblyAI**.

---

## 🔍 Overview

This application processes spoken audio, transcribes it, stores the transcription in a vector database, and enables natural language queries over that data. It combines cutting-edge components for transcription, semantic search, and generation:

### 📌 Workflow

1. **Audio Input**  
   Upload or stream an audio file into the system.

2. **Transcription**  
   The audio is transcribed to text using [**AssemblyAI**](https://www.assemblyai.com/), a state-of-the-art speech-to-text API.

3. **Vector Storage**  
   The transcription is embedded and stored in a **Qdrant** vector database for semantic retrieval.

4. **Contextual Retrieval**  
   On receiving a query, the system searches the vector DB for relevant segments of the transcribed audio.

5. **Response Generation**  
   Retrieved context is sent to **DeepSeek-R1**, a powerful LLM, to generate a coherent and informative response.

---

## 🛠️ Tech Stack

| Component       | Role                                                  |
|------------------|--------------------------------------------------------|
| **AssemblyAI**   | Transcribes speech into text using high-accuracy AI   |
| **Qdrant**       | Vector database for storing and retrieving embeddings |
| **DeepSeek-R1**  | LLM used to generate responses from retrieved context |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/audio-rag-deepseek.git
cd audio-rag-deepseek
