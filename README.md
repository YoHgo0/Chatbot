# Chatbot
Semantic search system that processes PDFs into embeddings and stores them in Pinecone for efficient retrieval

# PDF Semantic Search with Pinecone & OpenAI Embeddings

This project demonstrates an **end-to-end pipeline** for semantic search on PDF documents using:
- [LangChain](https://python.langchain.com) for text splitting and preprocessing
- [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) for vector representations
- [Pinecone](https://docs.pinecone.io/) as the vector database

---

## 🚀 Features
- **PDF ingestion** with `PyPDFLoader`
- **Chunking & Overlap** to handle long documents (e.g., chunk size 60, overlap 15) for context preservation
- **Embeddings generation** via `text-embedding-3-large` or `text-embedding-3-small`
- **Vector upsert** into Pinecone with unique `UUID` identifiers
- **Batch uploads** to respect API rate limits
- **Semantic search queries** with top-k results and metadata (page, source)

---
