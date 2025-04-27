# Finance_AI_Agent_v2

This notebook upgrades the financial agent into a **Retrieval-Augmented Generation (RAG) based AI Assistant** that can intelligently answer finance-related questions based on PDF documents and a vector database.

## Methodology
- **PDF-Based Knowledge Extraction**: Indexes and retrieves context from documents.
- **RAG Pipeline**: Combines retrieval and LLM-based answering.
- **Local Vector Database**: Stores document embeddings using PgVector.

## Tools & Libraries
- **Groq API** (LLM inference)
- **Agno Framework** (Agent setup)
- **PgVector** (vector database backend)
- **Sentence Transformers** (text embeddings)
- **Pypdf** (PDF reading)

## Implementation Steps
1. Install all dependencies (PgVector, Sentence Transformers, Agno, Groq).
2. Parse and embed finance-related PDFs into a vector store.
3. Implement retrieval logic to fetch top-k relevant chunks.
4. Construct RAG-based prompts combining retrieved context + query.
5. LLM (Groq model) answers using augmented context.
