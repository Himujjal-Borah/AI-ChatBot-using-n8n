# 🧠 AI Knowledge Base & Chatbot (RAG System using n8n + Pinecone + Gemini)

An advanced **Retrieval-Augmented Generation (RAG)** system built using **n8n**, where documents are automatically ingested from Google Drive, converted into embeddings, stored in **Pinecone**, and later used by an **AI chatbot** to answer user queries intelligently.

---

## 🚀 Features

- 📂 Auto-detect new files in Google Drive
- ⬇️ Download and process documents
- 🔍 Convert documents into vector embeddings
- 🧠 Store knowledge in Pinecone Vector Database
- 💬 AI chatbot with memory
- 📚 Context-aware responses using RAG
- ⚡ Real-time knowledge retrieval

---

## 🛠 Tech Stack

- **n8n** – Workflow automation  
- **Google Drive API** – File monitoring & retrieval  
- **Google Gemini Embeddings** – Vector generation  
- **Pinecone** – Vector database  
- **LangChain Agent** – AI orchestration  
- **Gemini Chat Model** – Conversational AI  
- **Memory Buffer** – Context retention  

---

## 📂 Workflow 1: Data Ingestion Pipeline

### 🔄 Flow

1. Google Drive Trigger monitors a folder  
2. New file is uploaded  
3. File is downloaded  
4. Document is processed using Data Loader  
5. Text is converted into embeddings  
6. Embeddings stored in Pinecone  

---

### 🧩 Nodes Used

- **Google Drive Trigger** → Detect new files  
- **Google Drive (Download)** → Fetch file  
- **Default Data Loader** → Extract content  
- **Gemini Embeddings** → Convert text → vectors  
- **Pinecone Vector Store** → Store embeddings  

---

## 💬 Workflow 2: AI Chatbot (RAG)

### 🔄 Flow

1. User sends chat message  
2. AI Agent receives query  
3. Memory provides conversation context  
4. Pinecone retrieves relevant documents  
5. AI generates answer using retrieved knowledge  

---

### 🧩 Nodes Used

- **Chat Trigger** → Receive user query  
- **AI Agent** → Orchestrates response  
- **Gemini Chat Model** → Generate answer  
- **Memory Buffer** → Maintain chat history  
- **Pinecone Vector Store (Tool)** → Retrieve knowledge  
- **Gemini Embeddings** → Query embedding  

---

## 🧠 How RAG Works

1. Documents → Converted into embeddings  
2. Stored in vector database (Pinecone)  
3. User asks a question  
4. System retrieves most relevant chunks  
5. AI generates answer using retrieved context  

---


---

## ⚙️ Setup Instructions

### 1️⃣ Import Workflows
- Import both Workflow 3 & Workflow 4 in n8n  

---

### 2️⃣ Configure Credentials

- Connect **Google Drive**
- Add **Pinecone API Key**
- Add **Google Gemini API**

---

### 3️⃣ Run System

- Upload documents to Google Drive folder  
- Activate ingestion workflow  
- Start chatbot workflow  
- Ask questions based on your documents  

---

## 🔥 Use Cases

- 📄 Personal knowledge base (CV, notes, docs)  
- 🤖 AI resume assistant  
- 🧑‍💼 Company knowledge chatbot  
- 📚 Study assistant  
- 💬 Customer support bot  

---

## 🚧 Future Improvements

- 📑 Support PDF, DOCX, CSV parsing enhancements  
- 🌐 Web UI chatbot (React frontend)  
- 🔐 Role-based access system  
- 📊 Analytics dashboard  
- 🤖 Multi-agent RAG system  

---

## 👨‍💻 Author

**Himujjal Borah**

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---

## 📜 License

This project is open-source and free to use.
