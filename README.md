# my-rag-project


# PDF RAG Chatbot with LangChain and Gemini

A Retrieval Augmented Generation (RAG) chatbot built with Python that allows users to ask questions about PDF documents.

The application processes a PDF document, converts the content into searchable vector embeddings, stores them in a ChromaDB vector database, and uses Google Gemini to generate accurate answers based on the retrieved information.

## Features

- Load and process PDF documents
- Split large documents into smaller text chunks
- Generate embeddings using Google Gemini Embeddings
- Store embeddings using ChromaDB vector database
- Retrieve relevant document sections using similarity search
- Generate answers using Google Gemini LLM
- Interactive command-line chatbot experience

## RAG Architecture

The application follows a Retrieval Augmented Generation pipeline:

1. **Document Loading**
   
   The PDF document is loaded using LangChain's `PyPDFLoader`.

2. **Text Chunking**

   The document is divided into smaller sections using `RecursiveCharacterTextSplitter`.

3. **Embedding Generation**

   Text chunks are converted into vector embeddings using:

   - Google Gemini Embeddings

4. **Vector Storage**

   The embeddings are stored and searched using:

   - ChromaDB

5. **Retrieval + Generation**

   When a user asks a question:

   - Relevant document chunks are retrieved
   - The context is passed to Gemini
   - Gemini generates a concise answer based on the document

## Technologies Used

- Python
- LangChain
- Google Gemini API
- ChromaDB
- Google Generative AI Embeddings
- Vector Databases
- Retrieval Augmented Generation (RAG)

## Project Structure

