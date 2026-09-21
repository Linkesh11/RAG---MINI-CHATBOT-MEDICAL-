# RAG---MINI-CHATBOT-MEDICAL-
An AI-powered Medical Eye Care Chatbot using RAG to answer eye-related medical queries based on trusted medical documents.


# Medical Eye Care RAG Chatbot

## Project Overview

The Medical Eye Care RAG Chatbot is an AI-powered question-answering system that uses Retrieval-Augmented Generation (RAG) to provide information about common eye diseases and their management.

The system retrieves relevant information from a medical PDF document and generates answers using the Qwen2.5-1.5B-Instruct language model.

This project demonstrates how Large Language Models (LLMs), vector databases, and semantic search can be combined to build a domain-specific medical chatbot.

## Features

- Loads medical information from PDF documents.
- Splits documents into smaller text chunks.
- Performs semantic similarity search.
- Generates context-based answers using an LLM.
- Focuses on common eye diseases and their management.
- Supports interactive question-answering through a Jupyter Notebook.

## Technologies Used

- Programming Language: Python
- Framework: LangChain
- Document Loader: PyPDFLoader
- Text Splitter: RecursiveCharacterTextSplitter
- Embedding Model: sentence-transformers/all-MiniLM-L6-v2
- Vector Database: FAISS
- Language Model: Qwen/Qwen2.5-1.5B-Instruct
- LLM Integration: Hugging Face Transformers
- Development Environment: Jupyter Notebook

## RAG Workflow

1. Load the medical eye-care PDF document.
2. Split the document into smaller chunks.
3. Generate embeddings for the text chunks.
4. Store the embeddings in a FAISS vector database.
5. Retrieve the three most relevant chunks for a user query.
6. Combine the retrieved context with the user's question.
7. Generate an answer using the Qwen language model.

## Project Configuration

- Chunk Size: 500 characters
- Chunk Overlap: 100 characters
- Retrieval Method: Similarity Search
- Number of Retrieved Documents: 3
- Generation Model: Qwen2.5-1.5B-Instruct

## Example Queries

- What are the physiology of the eye?
- What are common eye diseases?
- What are the symptoms of eye diseases?
- What are the management methods for eye diseases?

The answers depend on the information available in the source document.

## Project Structure

```text
Medical-Eye-Care-RAG-Chatbot/
|
|-- rag_2(1).ipynb
|-- Common Eye Diseases and their Management.pdf
|-- README.md
|-- requirements.txt
```

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Medical-Eye-Care-RAG-Chatbot.git
```

### 2. Navigate to the Project Directory

```bash
cd Medical-Eye-Care-RAG-Chatbot
```

### 3. Install Required Libraries

```bash
pip install torch
pip install -U langchain langchain-community langchain-text-splitters langchain-huggingface
pip install pypdf transformers sentence-transformers faiss-cpu
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook and run the cells in order.

Update the PDF file path in the notebook according to your local directory.

## Medical Disclaimer

This chatbot is intended for educational and informational purposes only.

It is not a medical diagnostic tool and does not replace professional medical advice. Consult a qualified eye-care professional for medical concerns.

## Future Enhancements

- Develop a Streamlit-based chatbot interface.
- Deploy the application as a web application.
- Improve retrieval accuracy using advanced RAG techniques.
- Add support for multiple medical documents.
- Implement conversation history.
- Add multilingual support.

## Author

Linkesh Mani

GitHub: https://github.com/your-username
