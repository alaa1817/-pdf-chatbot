# 📄 PDF Chatbot — RAG-Powered Q&A
A conversational AI app that lets you upload any PDF and ask questions about it in any language — powered by RAG (Retrieval Augmented Generation).

## 🌐 Live Demo
[pdf-chatbot88.streamlit.app](https://pdf-chatbot88.streamlit.app)

## 📌 Overview
This project implements a full RAG pipeline that retrieves relevant context from uploaded documents and uses a Large Language Model to generate accurate, context-aware answers — eliminating hallucinations from general LLM knowledge.

## ⚙️ How It Works
1. User uploads any PDF document
2. Document is split into chunks and converted to embeddings using **Sentence Transformers**
3. Embeddings are stored in a **FAISS** vector database
4. User asks a question in any language
5. System retrieves the most relevant chunks via similarity search
6. **Llama-3.1** (via Groq API) generates an answer based only on the document

## 🛠️ Tech Stack
- **RAG Framework:** LangChain
- **Embeddings:** Sentence Transformers (all-MiniLM-L6-v2)
- **Vector Database:** FAISS
- **LLM:** Groq API, Llama-3.1
- **Document Processing:** PyPDF, LangChain Text Splitters
- **Deployment:** Streamlit Cloud

## 📁 Project Structure
```
├── app.py               # Streamlit web app
├── requirements.txt     # Dependencies
└── README.md
```

## 🚀 Run Locally
```bash
git clone https://github.com/alaa1817/pdf-chatbot
cd pdf-chatbot
pip install -r requirements.txt
streamlit run app.py
```

## 📬 Contact
**Alaa Ibrahim** — [LinkedIn](https://linkedin.com/in/alaa-jadallah-484a4a2a8) | [GitHub](https://github.com/alaa1817)

