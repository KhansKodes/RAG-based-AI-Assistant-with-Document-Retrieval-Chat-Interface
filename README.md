# 🔍 Supabase RAG AI Agent – Document Q&A with OpenAI + n8n + Google Drive

This project is a complete **Retrieval-Augmented Generation (RAG) pipeline** that allows users to upload documents to Google Drive and interact with them via a chat interface powered by **OpenAI**, **n8n**, and **Supabase**.

## ✨ Features

- 📥 **Auto-ingest documents** from a specific Google Drive folder (triggered on file upload or update)
- 🧠 **Extract and chunk document content** using LangChain's Recursive Text Splitter
- 🤖 **Generate vector embeddings** using OpenAI’s `text-embedding-3-small` model
- 🗄️ **Store embeddings in Supabase vector store** for fast semantic retrieval
- 💬 **Context-aware Q&A** using a GPT-4o-mini powered chat interface
- 💾 **Chat memory** powered by Postgres for continuous, multi-turn conversations
- 🔁 Fully automated with **n8n workflows**

---

## 🧠 Use Case

> Want to query your meeting notes, legal docs, or knowledge base using natural language?  
This project enables real-time chat with your own documents — just upload, ask, and get contextually accurate answers.

---

## 🛠 Tech Stack

- [n8n](https://n8n.io/) – workflow automation
- [Supabase](https://supabase.com/) – vector database + Postgres
- [OpenAI](https://openai.com/) – embeddings + GPT-4o-mini
- [LangChain](https://www.langchain.com/) – document loaders, memory, and tools
- [Google Drive API](https://developers.google.com/drive) – document triggers & downloads

---

## 🧩 Workflow Overview

1. ✅ **User uploads/updates a doc to Google Drive**
2. 🔁 n8n triggers on file creation/update
3. 📄 File is downloaded and text is extracted
4. ✂️ Text is chunked and embedded via OpenAI
5. 📦 Embeddings are stored in Supabase with metadata
6. 💬 User sends chat query → relevant chunks retrieved
7. 🧠 GPT-4o-mini uses RAG to generate an accurate response

---
## 📸 Screenshots

![image](https://github.com/user-attachments/assets/17efbae0-8056-4b60-9c43-9f6cead8d33d)

![image](https://github.com/user-attachments/assets/d5e321da-23b7-4511-83f4-a1e5bd64691d)



