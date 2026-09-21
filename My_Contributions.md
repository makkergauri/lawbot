# My Contributions

This is a fork of [aarul-kumar/lawbot](https://github.com/aarul-kumar/lawbot),
a team project. This file covers only the parts I worked on.

## What I worked on

### Document processing and vector search (`vector_database.py`)
- Built PDF ingestion and text extraction using PDFPlumber
- Implemented recursive chunking with overlap to improve retrieval quality
- Generated embeddings with Ollama (`nomic-embed-text`) and stored them in a
  persistent FAISS index

### RAG pipeline and LLM integration (`rag_pipeline.py`)
- Implemented Top-K similarity retrieval and context aggregation
- Designed the structured prompt that keeps answers grounded in the document
  and returns a fallback ("I don't know based on the provided document.")
  when the answer isn't in the context
- Integrated the configurable LLM backend: local (Ollama) and cloud (Groq)

### Frontend (`frontend.py`)
- Built the Streamlit interface for uploading PDFs and asking questions

### Other
- Testing, documentation, sample documents, research, debugging, etc.

## Tech used
Python, LangChain, FAISS, Ollama, Groq API, PDFPlumber, Streamlit
