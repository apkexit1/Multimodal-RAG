# Multimodal RAG Pipeline

An end-to-end Multimodal Retrieval-Augmented Generation (RAG) system designed to process, index, and query unstructured documents containing text, embedded images, and tables (such as financial reports and technical PDFs).

## 🚀 Key Features

* **Multimodal Extraction:** Parses text, extracts embedded images, and structures tabular data from complex PDF documents using `PyMuPDF`.
* **Vector Indexing & Retrieval:** Generates dense embeddings via Hugging Face (`sentence-transformers`) and indexes vector representations into a Pinecone vector database.
* **LLM Orchestration:** Powered by `LangChain` and `Groq` (Llama-3 models) for ultra-fast multi-modal reasoning and contextual generation.
* **Secure Key Management:** Implements `python-dotenv` for local environment variable isolation, preventing credential leaks.

## 🛠️ Tech Stack

* **Frameworks:** LangChain, LangChain-Core, LangChain-Groq, LangChain-Pinecone
* **Vector Database:** Pinecone
* **Embeddings:** Hugging Face (`sentence-transformers/all-MiniLM-L6-v2`)
* **LLM Engine:** Groq (Llama-3)
* **Document Processing:** PyMuPDF (`fitz`), Pillow, Pandas, Tabulate
* **Environment:** Python 3.12

## 📁 Repository Structure

```text
Multimodal_Rag/
│
├── Build_Multimodal_RAG.ipynb     # Main RAG execution notebook
├── NovaCore_Multimodal_Company_Report_2026.pdf # Sample document dataset
├── novacore_extracted_images/     # Extracted images directory
├── .env.example                   # Template for required environment variables
├── .gitignore                     # Git tracking exclusion rules
└── README.md                      # Project documentation
