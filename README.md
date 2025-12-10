# Context-Aware Document Question Answering System

This project is a context-aware Question Answering (QA) system that lets you ask natural language questions over your own documents (e.g. notes, textbooks, or technical PDFs). It combines transformer-based text embeddings with a FAISS vector index to retrieve relevant passages and an extractive QA model to generate precise answers.

---

## Overview

The system works in three main stages:

1. **Document Ingestion & Embedding**  
   Documents are preprocessed and converted into dense vector representations using a DistilBERT-based model.

2. **Vector Indexing with FAISS**  
   These embeddings are stored in a FAISS index to enable fast semantic search over large collections of documents.

3. **Question Answering**  
   When a user asks a question, it is embedded, the most relevant document chunks are retrieved from the FAISS index, and an extractive QA model is used to generate the final answer along with supporting context.

---

## Features

- 🔍 **Semantic search** over custom document collections  
- 🧠 **Transformer-based text embeddings** (DistilBERT)  
- ⚡ **Fast similarity search** using FAISS vector database  
- 💬 **Streamlit web interface** for interactive Q&A  
- 📎 **Answer with supporting context** (relevant passage)  
- 🧱 Modular code structure for training, indexing, and inference

(Planned / in progress – customize based on what you add)
- 💬 Chat-style multi-turn QA
- 📊 Confidence scores for each answer
- 🌐 Support for domain-specific or multilingual datasets

---

## Tech Stack

- **Language & Frameworks:** Python, PyTorch  
- **NLP:** Hugging Face Transformers, DistilBERT  
- **Vector Search:** FAISS (Facebook AI Similarity Search)  
- **Web UI:** Streamlit  
- **Utilities:** NumPy, Pandas, Scikit-learn  

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Boreddyakshithareddy3k/context-aware-document-qa.git
cd context-aware-document-qa
