# Moroccan Administrative AI Assistant

## Overview
Navigating administrative procedures in Morocco can often be complex and time-consuming due to scattered information and unclear requirements.

This project introduces an AI-powered assistant designed to simplify access to administrative information by enabling users to ask natural language questions about Moroccan administrative procedures.

The system is built as a Streamlit-based application and leverages Retrieval-Augmented Generation (RAG) to provide accurate and context-aware answers based on official documents.

---

## Features

- Ask questions about Moroccan administrative procedures (e.g., CNIE renewal, required documents, fees, and procedures)
- Context-aware responses using vector search over structured administrative documents
- Chat-style interface similar to ChatGPT for intuitive interaction
- Fast and relevant information retrieval using semantic search

---

## How It Works

The system follows a Retrieval-Augmented Generation (RAG) pipeline:

1. User submits a question in natural language  
2. The query is converted into embeddings using OpenAI models  
3. Relevant documents are retrieved from a FAISS vector database  
4. Retrieved context is passed to a language model (GPT-4o-mini)  
5. The model generates a final contextualized answer

---

## Tech Stack

- Python 3.12+
- Streamlit (web interface)
- LangChain (RAG pipeline orchestration)
- FAISS (vector similarity search)
- OpenAI API:
  - GPT-4o-mini (response generation)
  - text-embedding-3-small (embeddings)
- dotenv (secure API key management)

---

## Use Cases

- Understanding administrative procedures in Morocco
- Finding required documents for official requests
- Getting guidance on fees and steps for public services
- Reducing time spent searching official websites

---

## Project Goal

The goal of this project is to make administrative information more accessible, understandable, and interactive through the use of modern AI techniques such as LLMs and semantic search.

---

## Conclusion

This assistant demonstrates how Retrieval-Augmented Generation can significantly improve access to structured administrative knowledge by combining large language models with domain-specific document retrieval.
