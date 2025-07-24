# RAG Based PDF Question Answering 

A command-line based question-answering tool built using Python, LangChain, FAISS, and Gemini Pro. It extracts text from a PDF file, chunks it, indexes it using vector embeddings, and uses Google Gemini Pro to answer user queries based on the document content.

## Features
-> Extracts text from any PDF document

-> Splits large text into manageable chunks

-> Embeds chunks using HuggingFace Embeddings

-> Creates a vector store with FAISS for semantic similarity search

-> Uses Google Gemini Pro to answer questions based on the most relevant chunks

## Tech Stack
-> Python

-> LangChain (Text Splitters, FAISS Integration)

-> HuggingFace Embeddings

-> Google Gemini Pro (via google.generativeai)

-> PyPDF (for text extraction)

## How It Works
-> The tool reads and extracts all text from a given PDF using PyPDF.

-> The extracted text is split into overlapping chunks using RecursiveCharacterTextSplitter.

-> These chunks are converted into vector embeddings using HuggingFace Embeddings.

-> A FAISS vector store is created to enable fast similarity search.

-> When a user enters a question, the system retrieves the top relevant chunks.

-> The context from these chunks is sent to the Gemini Pro model along with the user query.

-> Gemini Pro generates a relevant and contextual answer.



