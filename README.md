# YouTube Video Summarizer & Q&A Chatbot (RAG-Based)

## Overview

This project is a Retrieval-Augmented Generation (RAG) based chatbot that allows users to interact with YouTube videos using natural language. Users can provide a YouTube video URL, generate a concise summary of the video's content, and ask questions related to the video. The chatbot retrieves relevant information from the video transcript and uses a Large Language Model (LLM) to generate accurate, context-aware responses.

## Features

* Extracts transcripts from YouTube videos using a video URL
* Generates concise video summaries
* Retrieval-Augmented Generation (RAG) based question answering
* Context-aware responses based on video content
* Interactive chat interface
* Efficient retrieval using vector embeddings

## Technologies Used

* Python
* Streamlit
* LangChain
* Google Gemini API / OpenAI API
* YouTube Transcript API
* FAISS Vector Database
* Hugging Face Embeddings
* NLP Techniques

## How It Works

1. User provides a YouTube video URL.
2. Transcript is extracted using YouTube Transcript API.
3. Transcript is split into smaller chunks.
4. Text chunks are converted into vector embeddings.
5. Embeddings are stored in a FAISS vector database.
6. Relevant transcript chunks are retrieved based on the user's query.
7. The LLM generates answers using retrieved context (RAG pipeline).
8. Users can view summaries or ask questions about the video.

## Architecture

```
YouTube URL
     ↓
Transcript Extraction
     ↓
Text Chunking
     ↓
Embeddings Generation
     ↓
FAISS Vector Store
     ↓
Retriever
     ↓
LLM (Gemini/OpenAI)
     ↓
Summary / Q&A Response
```



## Installation

```bash
git clone <repository-url>
cd YouTube-RAG-Chatbot
pip install -r requirements.txt
```

## Run the Project

```bash
streamlit run app.py
```

## Sample Use Case

Input:

```
YouTube URL:
https://youtube.com/...
```

User Query:

```
What are the main points discussed in the video?
```

Output:

```
The video discusses...
```

## Key Concepts

* Retrieval-Augmented Generation (RAG)
* Natural Language Processing (NLP)
* Vector Embeddings
* Semantic Search
* Large Language Models (LLMs)

## Future Enhancements

* Multi-video knowledge base
* Chat history and memory
* Support for multilingual transcripts
* PDF export of summaries
* Advanced semantic search

## Conclusion

This project demonstrates the integration of NLP, vector databases, and Large Language Models to create an intelligent YouTube assistant capable of summarizing videos and answering user questions with high contextual accuracy using a RAG-based architecture.
