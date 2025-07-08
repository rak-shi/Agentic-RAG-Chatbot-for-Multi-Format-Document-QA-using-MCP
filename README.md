# Agentic-RAG-Chatbot-for-Multi-Format-Document-QA-using-MCP
A chatbot capable of answering user queries from uploaded PDFs, DOCX, PPTX, CSV, and TXT/MD using an agent-based architecture with Retrieval-Augmented Generation and Model Context Protocol for agent communication.
## 🚀 Features

✅ Multi-format document ingestion: **PDF, DOCX, PPTX, CSV, TXT**  
✅ Agentic architecture:
- **IngestionAgent:** parses and preprocesses documents
- **RetrievalAgent:** generates embeddings, performs semantic retrieval
- **LLMResponseAgent:** formats GPT queries using retrieved context, returns grounded answers

✅ Uses **FAISS + sentence-transformers** for retrieval  
✅ Uses **OpenAI GPT** for answer generation  
✅ **Gradio UI** for seamless upload, querying, and response viewing

---

## 🛠️ Tech Stack

- Python
- FAISS
- sentence-transformers (HuggingFace)
- OpenAI GPT
- Gradio (UI)
- PyMuPDF, python-docx, python-pptx, pandas (parsing)
- Google Colab / local Python

## 🚀 Usage

✅ **On Google Colab**:
- Open `app.ipynb`
- Upload your documents (PDF, DOCX, PPTX, CSV, TXT)
- Enter your questions
- View GPT-based answers with retrieved context

✅ **Locally (optional):**
If you prepare `app.py`, run:
```bash
python app.py
```
It will launch a **Gradio UI** in your browser.
## 🧩 Challenges Faced

- Managing consistent chunking for diverse document formats.
- Preserving context relevance during retrieval while respecting GPT token limits.
- Building a lightweight UI that integrates cleanly with Colab for easy evaluation.
## 🚀 Future Improvements

- Add multi-turn conversational memory.
- REST API endpoints for integration.
- Highlight source snippets in GPT answers.
- Offline embeddings generation for reduced API costs.


