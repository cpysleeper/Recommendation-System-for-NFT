# 🔍 NFT Retriever System

This project implements a **semantic search system** for NFT collections using the [multilingual-e5-large-instruct](https://huggingface.co/intfloat/multilingual-e5-large-instruct) model and dense vector search with [FAISS](https://github.com/facebookresearch/faiss). It enables natural language queries to retrieve the most relevant NFTs based on their descriptions.

---

## 📁 Project Overview

- **Input:** NFT collection metadata (JSON files)
- **Output:** Searchable CSV with `document_id`, `title`, and `text`
- **Model:** SentenceTransformer (E5)
- **Indexing:** FAISS for top-k dense retrieval
- **Hardware:** Apple M2 GPU used via PyTorch MPS backend

---

## ⚙️ Features

- Multilingual text embedding with E5 model
- FAISS-based dense retrieval
- Query-NFT matching with natural language input
- GPU-accelerated embedding generation on Apple Silicon

---

## 🚀 Getting Started

1. **Install dependencies**
   ```bash
   pip install sentence-transformers faiss-cpu pandas
