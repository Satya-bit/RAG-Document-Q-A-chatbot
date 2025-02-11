# RAG-Document-Q-A-chatbot
This project implements a Retrieval-Augmented Generation (RAG) pipeline for document-based question answering (Q&amp;A) using LangChain, Ollama, and FAISS. Users can upload research papers (PDFs), which are processed into vector embeddings, enabling an AI model to retrieve relevant content and generate accurate responses.

🚀 Features
🔍 Document Ingestion: Loads and processes PDFs using PyPDFDirectoryLoader.
📝 Text Splitting: Breaks down documents into chunks for efficient retrieval.
🧠 Vector Embeddings: Utilizes OllamaEmbeddings() for text representation.
🗂 FAISS Indexing: Stores document embeddings for fast and efficient similarity search.
🗨 Chat Interface: Users can ask questions, and the system retrieves relevant document sections before generating responses.
🎛 Streamlit UI: Interactive front-end for model selection, temperature control, and response tuning.
🛠 Tech Stack
LangChain (for chaining LLM queries)
Ollama (for generating embeddings and LLM responses)
FAISS (for vector search)
PyPDFLoader (for document parsing)
Streamlit (for building the UI)
💡 How It Works
Document Ingestion: Load PDFs from /research_papers directory.
Text Processing: Split documents into smaller chunks for better retrieval.
Vectorization: Convert text into embeddings using OllamaEmbeddings().
Indexing: Store embeddings in FAISS for efficient retrieval.
Query Processing: User questions are embedded and compared against the document index to retrieve the most relevant context.
Response Generation: The model answers based on retrieved content.
