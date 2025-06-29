# Gen_AI_Doc

# AI-Assistant

# 🤖 GenAI Doc Assistant #

Turn any PDF/TXT document into an intelligent Q&A and challenge generator using GenAI & vector search.

# 🚀 Features #

- Upload PDF/TXT documents
- Chunking + vector embeddings via `FAISS`
- Contextual question generation (Easy / Medium / Hard)
- LLM-powered answers using Hugging Face Transformers

# 📐 Architecture #

1. Text Extraction: `PyMuPDF` for PDF / native for TXT
2. Chunking & Embedding:
   - Recursive text splitting
   - sentence-transformers via `HuggingFaceEmbeddings`
3. Vector DB: `FAISS` for fast semantic search
4. LLM Q&A Generator:
   - Prompt-tuned `flan-t5-large` model using `HuggingFacePipeline`

#🧠 Reasoning Flow #

plaintext
[Document Upload]
        ↓
[Text Extraction]
        ↓
[Split + Embed + Store]
        ↓
[Select Difficulty Level]
        ↓
[Generate Challenge + Answer using LLM]
