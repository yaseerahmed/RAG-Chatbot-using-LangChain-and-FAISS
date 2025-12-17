# RAG-Chatbot-using-LangChain-and-FAISS
end-to-end Retrieval-Augmented Generation (RAG) system using LangChain, FAISS, and HuggingFace embeddings to enable semantic document search and context-aware LLM responses with Groq LLaMA-3.1.

End-to-End RAG System with FAISS, LangChain & LLaMA-3.1
Project Overview

This project implements a Retrieval-Augmented Generation (RAG) system for semantic document search and context-aware question answering.
It demonstrates an end-to-end pipeline:

Document loading and chunking

Embedding generation with HuggingFace sentence-transformers

Vector storage and retrieval using FAISS

LLM-based response generation using Groq-hosted LLaMA-3.1

The system ensures accurate, context-grounded answers and handles real-world issues like LangChain API updates and model deprecation.

Features

Semantic Search: Retrieve most relevant chunks using vector similarity

Context-Aware Answers: RAG system provides grounded responses based on retrieved text

FAISS Vector Database: Fast and scalable similarity search

Secure API Handling: Loads LLM API keys from .env

Production-Ready: Handles errors, API changes, and model deprecation

Tech Stack

Python 3.13

LangChain – for RAG orchestration

FAISS – for vector similarity search

HuggingFace Embeddings – sentence-transformers/all-MiniLM-L6-v2

Groq LLaMA-3.1 – for LLM responses

.env – for secure API key storage

Getting Started
1. Clone the repository
git clone https://github.com/yourusername/rag-faiss-langchain.git
cd rag-faiss-langchain

2. Install dependencies
pip install -r requirements.txt

3. Add API keys

Create a .env file:

GROQ_API_KEY=your_groq_api_key_here

4. Run indexing (create FAISS vector store)
python rag_index.py

5. Query the system
python rag_query.py


Example query:
"What is this document about?"

Output: Context-grounded answer from the indexed documents
"What is this document about?"

Output: Context-grounded answer from the indexed documents
