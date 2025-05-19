# 🏥 AI-Powered Healthcare Assistant using RAG and GPT-4

This project introduces a **Retrieval-Augmented Generation (RAG)** based AI assistant designed to enhance how **patients and doctors interact with unstructured medical records**. By combining **Large Language Models (LLMs)**, **semantic search**, and intelligent document processing, the system delivers **personalized, role-specific insights** from past medical history.

---

## 🚀 Features

- 🔍 **Semantic Search:** Efficiently retrieves relevant medical history using vector embeddings.
- 💬 **LLM-Powered Q&A:** Answers questions based on retrieved context using GPT-4 or other LLMs.
- 🧠 **Role-Specific Output:** Simplified summaries for patients and detailed context for healthcare professionals.
- 📄 **Document Ingestion:** Parses PDF medical reports (lab results, diagnoses, prescriptions, etc.).
- 📦 **ChromaDB Integration:** Uses a vector database for fast and accurate chunk retrieval.
- ⚙️ **Scalable & Modular Design:** Built to support expansion across users, roles, and medical domains.

---

## 🧱 Tech Stack

| Component | Description |
|----------|-------------|
| `Python` | Core language |
| `LangChain` | Orchestration and LLM interfacing |
| `ChromaDB` | Vector database for semantic search |
| `SentenceTransformers` | Embedding model for vectorization |
| `OpenAI GPT-4` | LLM for generating contextual responses |
| `PyMuPDF / pdfminer` | PDF parsing and text extraction |
| `Streamlit` (optional) | Frontend UI for interaction (if implemented) |

---

## 📁 Project Structure


---

## 📌 How It Works

1. **Upload Medical Records:** Accepts PDF files containing medical history (lab reports, prescriptions, etc.).
2. **Parse & Chunk Text:** Extracts text, tokenizes, and chunks documents into manageable sizes.
3. **Embed Chunks:** Uses sentence transformers to convert each chunk into a vector representation.
4. **Store in Vector DB:** Saves all vectors into ChromaDB for future retrieval.
5. **Query Interface:** User inputs a query; the system retrieves the top-k relevant chunks.
6. **LLM Response:** Retrieved chunks + query are passed to GPT-4 to generate a coherent answer.
7. **Role-Aware Output:** Formats the response based on the user's role (doctor vs. patient).

---

## 📦 Installation

1. **Clone the repo:**
   ```bash
   git clone https://github.com/your-username/healthcare-rag-assistant.git
   cd healthcare-rag-assistant
