# universal-pdf-assistant

## Overview
Universal PDF RAG System is an intelligent document analysis tool that leverages Qwen2.5 LLM and Retrieval-Augmented Generation (RAG) to answer questions about your PDF documents. It features a modern Streamlit web interface for easy document upload and querying.

## Features
- PDF text extraction and chunking
- Semantic search with vector database (FAISS)
- Qwen2.5 LLM for contextual answers
- Streamlit web UI for uploads and queries
- Response refinement for high-quality answers

## Usage Instructions

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Start the Application
You can run the system in two main ways:

#### Option A: Production/CLI Startup
```bash
python startup.py
```

#### Option B: Streamlit Web Interface
```bash
streamlit run streamlit_app.py --server.port 8501
```

### 3. Using the System
1. **Upload PDFs**: Use the web interface to upload your PDF documents.
2. **Processing**: The system extracts text and creates vector embeddings automatically.
3. **Ask Questions**: Enter your questions about the uploaded documents in the web UI.
4. **Get Answers**: The system retrieves relevant content and generates intelligent answers using Qwen2.5 LLM.

## Deployment
- For Heroku or cloud deployment, see `README_DEPLOYMENT.md` for detailed instructions and configuration notes.

## File Structure
- `streamlit_app.py`: Main web app
- `startup.py`: Production startup script
- `rag_system.py`: Core RAG logic
- `enhanced_vector_db/`: Vector database storage
- See `README_DEPLOYMENT.md` for a full breakdown

## Status
**DEPLOYMENT READY**

---
For advanced configuration, system details, and deployment options, refer to [README_DEPLOYMENT.md](./README_DEPLOYMENT.md).