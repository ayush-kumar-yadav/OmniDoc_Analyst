# 🔍 OmniDocAnalyst – AI-Powered Multi-Format Document Analysis with RAG & LLMs

OmniDocAnalyst is an AI-based document intelligence system that allows users to upload and interact with a wide variety of documents — including PDFs, Word files, Excel sheets, plain text, and images — using Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG).

It enables natural language question answering, summarization, and contextual analysis directly from your uploaded files.

---

## 🚀 Features

- 📄 **Supports Multiple File Types**: `.pdf`, `.docx`, `.txt`, `.xlsx`, `.csv`, and `.jpg/.png` images with text
- 🧠 **RAG Pipeline with LLMs**: Uses vector embeddings + LLMs to provide contextual answers
- 💬 **Ask Questions About Your Files**: Chatbot interface for querying document contents
- 🧾 **Summarization & Insights**: Automatically extracts summaries and key insights
- ⚙️ **Extensible Modular Backend**: Swap vector store, LLM, or chunking strategy easily
- 🌐 **Simple Web UI**: Built with Gradio (or Streamlit) for interactive use

---

## 📁 Supported File Formats

| File Type | Extraction Method |
|-----------|-------------------|
| `.pdf`    | PyMuPDF, pdfplumber |
| `.docx`   | python-docx        |
| `.csv`    | pandas             |
| `.xlsx`   | pandas (Excel engine) |
| `.txt`    | Built-in           |
| `.jpg/.png` | pytesseract (OCR) |

---

## 🛠️ Tech Stack

- **Backend**: Python, LangChain, ChromaDB, Hugging Face Transformers
- **LLMs**: OpenAI (GPT-4), Ollama (LLaMA, Mistral), Hugging Face models
- **Embeddings**: Sentence Transformers, OpenAI Embeddings
- **Frontend**: Gradio / Streamlit
- **OCR**: pytesseract
- **Document Parsing**: pdfplumber, PyMuPDF, python-docx, pandas

---


▶️ Usage
Run the App

bash
Copy
Edit
python app.py
Upload Document(s)

Ask questions like:

"Summarize this invoice"

"What is the total amount payable?"

"Extract all dates and customer names"

📌 Example Use Cases
📃 Contract or invoice QA system

📚 Academic or legal document summarization

🧾 Receipt and financial document analysis

📊 Business document assistant

📂 Project Structure

OmniDocAnalyst/
│
├── app.py                  # Main app entrypoint
├── extractors/             # Text extraction from different file types
│   ├── pdf_extractor.py
│   ├── word_extractor.py
│   └── ocr_image_extractor.py
├── rag_pipeline/           # Chunking, embeddings, vector search
│   └── rag_engine.py
├── llm_interface/          # OpenAI, Ollama, HuggingFace model wrappers
├── ui/                     # Gradio or Streamlit interface
├── requirements.txt
└── README.md
🔒 Disclaimer
This project is intended for educational and research use. Ensure compliance with data privacy regulations when uploading sensitive documents.

🤝 Contributions
Pull requests, feature requests, and feedback are welcome!

