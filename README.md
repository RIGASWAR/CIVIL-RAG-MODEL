# CIVIL-RAG-MODEL

AI-powered Civil Engineering Assistant built using Retrieval-Augmented Generation (RAG), FAISS Vector Search, Sentence Transformers, FastAPI, React, and Groq LLMs. The system enables engineers and students to upload technical documents, perform semantic search, analyze datasets, and receive source-grounded answers through an intelligent conversational interface.

---

## Features

- PDF, DOCX, and TXT document ingestion
- Retrieval-Augmented Generation (RAG) pipeline
- Semantic search using FAISS vector database
- Query expansion using Groq LLM
- Cross-Encoder reranking for improved retrieval quality
- Reflection-based answer validation
- Confidence scoring mechanism
- Source-grounded responses with citations
- Dataset analysis support for CSV files
- FastAPI backend with React frontend

---

## Architecture

```text
User Query
    ↓
Query Expansion (Groq LLM)
    ↓
Semantic Retrieval (FAISS)
    ↓
Cross-Encoder Reranking
    ↓
Context Assembly
    ↓
LLM Response Generation
    ↓
Reflection & Confidence Scoring
    ↓
Final Answer with Sources
```

---

## Key Features

### Intelligent Document Retrieval
- Converts uploaded engineering documents into semantic vector embeddings.
- Retrieves the most relevant document chunks based on meaning rather than keyword matching.

### Query Expansion
- Uses Groq-powered LLMs to generate alternative search queries.
- Improves retrieval accuracy for abbreviations, technical terminology, and domain-specific questions.

### Reranking Pipeline
- Uses Cross-Encoder models to rerank retrieved chunks.
- Ensures the most relevant context is sent to the language model.

### Reflection-Based Validation
- Evaluates generated answers before returning them.
- Improves factual consistency and reliability.

### Dataset Analytics
- Supports CSV datasets for engineering data analysis.
- Enables users to ask questions about uploaded structured data.

---

## Performance

- Indexed **1600+ semantic chunks**
- Supports **multi-document retrieval**
- Uses **FAISS IVFFlat indexing**
- Hybrid retrieval + reranking architecture
- Source-aware answer generation
- FastAPI REST API backend
- React-based conversational UI

---

## Tech Stack

### Backend
- Python
- FastAPI
- FAISS
- Sentence Transformers
- Groq API
- NumPy
- Pandas

### Frontend
- React.js
- JavaScript
- HTML5
- CSS3

### AI / NLP
- Retrieval-Augmented Generation (RAG)
- Semantic Search
- Query Expansion
- Cross-Encoder Reranking
- Reflection Framework

---

## Screenshots

### Home Page

<img src="screenshots/home-page.png" width="900"/>

### Document Upload & Indexing

<img src="screenshots/document-upload.png" width="900"/>

### AI Question Answering

<img src="screenshots/answer-demo.png" width="900"/>

### Advanced RAG Query

<img src="screenshots/advanced-rag-demo.png" width="900"/>

### Recommendation Generation

<img src="screenshots/recommendation-demo.png" width="900"/>

---

## Installation

### Clone Repository

```bash
git clone https://github.com/RIGASWAR/CIVIL-RAG-MODEL.git
cd CIVIL-RAG-MODEL
```

### Backend Setup

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

pip install -r ../requirements.txt
```

### Configure Environment Variables

Create a `.env` file inside the backend folder:

```env
GROQ_API_KEY=your_groq_api_key
```

### Run Backend

```bash
python run.py
```

Backend runs at:

```text
http://localhost:8000
```

### Frontend Setup

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

## Example Queries

- What is water cement ratio?
- Explain Ordinary Portland Cement (OPC).
- How does water cement ratio affect concrete strength?
- Recommend ways to improve concrete durability.
- Analyze the uploaded concrete strength dataset.
- Summarize the uploaded tender document.

---

## Future Enhancements

- Multi-user authentication
- Cloud deployment
- Chat history persistence
- Hybrid keyword + vector search
- Advanced engineering dataset analytics
- Support for additional engineering domains

---

## Author

**Rigaswar S**

B.Tech Information Technology  
PSG College of Technology

GitHub: https://github.com/RIGASWAR