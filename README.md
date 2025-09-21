###TRADITIONAL RAG PIPELINE 

This project implements a Retrieval-Augmented Generation (RAG) pipeline for working with PDFs and text files. It uses:

LangChain for document loading and chunking

SentenceTransformers for embeddings

ChromaDB as the vector database

A custom RAGRetriever class for query-based retrieval

The pipeline lets you load documents (PDFs, text files), split them into smaller chunks, embed them, store them in a persistent vector database, and retrieve relevant chunks for any query.

⚙️ Features

Load PDFs and text files automatically from a directory

Clean & customizable metadata injection (e.g., source file, file type, page number)

Split long documents into overlapping chunks for better context retrieval

Generate sentence embeddings using HuggingFace’s all-MiniLM-L6-v2 (or any SentenceTransformer model)

Store and query embeddings in a persistent ChromaDB collection

Retrieve documents using a custom retriever that returns text, metadata, and similarity scores
