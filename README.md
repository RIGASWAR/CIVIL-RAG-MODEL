# CIVIL-RAG-MODEL – AI-Powered Civil Engineering Assistant

An intelligent Retrieval-Augmented Generation (RAG) system designed for Civil Engineering professionals and students. The platform combines semantic search, vector embeddings, reranking models, and Large Language Models (LLMs) to provide accurate, context-aware answers from technical documents and datasets.

---

## Overview

CIVIL-RAG-MODEL enables users to upload civil engineering documents and interact with them through a conversational AI interface.

The system retrieves relevant information from technical documents, standards, reports, and datasets, then generates contextual responses using advanced language models.

---

## Features

* Retrieval-Augmented Generation (RAG) pipeline
* Semantic document search using vector embeddings
* AI-powered question answering
* PDF, DOCX, and TXT document support
* Dataset-based querying and analysis
* Reranking for improved retrieval accuracy
* React-based interactive user interface
* FastAPI backend services
* Civil engineering domain specialization

---

## Architecture

```text
User Query
     │
     ▼
React Frontend
     │
     ▼
FastAPI Backend
     │
     ▼
Query Expansion
     │
     ▼
Vector Search (Embeddings)
     │
     ▼
Reranking Model
     │
     ▼
LLM Response Generation
     │
     ▼
Context-Aware Answer
```

---

## Project Structure

```text
CIVIL-RAG-MODEL/
│
├── backend/
│   ├── civil_rag/
│   │   ├── api.py
│   │   ├── vectorstore.py
│   │   ├── query_expander.py
│   │   ├── reranker.py
│   │   ├── router.py
│   │   ├── generator.py
│   │   └── ingest.py
│   │
│   ├── data/
│   ├── datasets/
│   ├── vectorstore/
│   └── run.py
│
├── frontend/
│   └── civil-rag-ui/
│
└── requirements.txt
```

---

## Tech Stack

### Backend

* Python
* FastAPI
* Uvicorn

### AI & NLP

* Retrieval-Augmented Generation (RAG)
* Sentence Transformers
* Vector Embeddings
* Semantic Search
* Cross-Encoder Reranking
* Groq LLM API

### Frontend

* React.js
* JavaScript
* CSS

### Data Processing

* Pandas
* PDF/Text Parsing
* Document Chunking

---

## Installation

### Clone Repository

```bash
git clone https://github.com/RIGASWAR/CIVIL-RAG-MODEL.git
cd CIVIL-RAG-MODEL
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file inside the backend directory.

```env
GROQ_API_KEY=your_api_key_here
```

---

## Run Backend

```bash
cd backend
python run.py
```

Backend runs at:

```text
http://localhost:8000
```

---

## Run Frontend

```bash
cd frontend/civil-rag-ui
npm install
npm start
```

Frontend runs at:

```text
http://localhost:3000
```

---

## Use Cases

* Civil Engineering Document Search
* Technical Standards Assistance
* Construction Technology Queries
* Dataset Exploration
* Educational Learning Support
* Intelligent Knowledge Retrieval

---

## Future Enhancements

* Multi-document chat
* PDF report generation
* User authentication
* Cloud deployment
* Advanced analytics dashboard
* Hybrid retrieval techniques

---

## Author

RIGASWAR S

B.Tech Information Technology
PSG College of Technology

---

## License

This project is licensed under the MIT License.
