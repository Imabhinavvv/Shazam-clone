# Enhancing Search Engine Relevance for Video Subtitles (Like Shazam for Subtitles)

## Overview
Finding the right information in video subtitles can be tricky. This project improves search relevance by using AI to better understand subtitles, making them more accessible and searchable.

## Goal
Build a smart search engine that retrieves relevant subtitles based on user queries. We use **Natural Language Processing (NLP)** and **Machine Learning (ML)** to improve accuracy and relevance.

## Keyword vs. Semantic Search
- **Keyword-Based Search**: Matches exact words but lacks deep understanding.
- **Semantic Search**: Understands meaning using AI-based embeddings, providing better results.

## How It Works
1. **Process Subtitles**:
   - Extract subtitle text from a **.db** file.
   - Clean data by removing timestamps and unwanted characters.
   - Convert text into numerical representations (embeddings).
   - Store embeddings in **ChromaDB** for fast retrieval.

2. **User Query Matching**:
   - Accepts **audio input** from the user.
   - Converts speech to text using **AssemblyAI**.
   - Converts text into embeddings using **SentenceTransformers**.
   - Calculates **cosine similarity** to find the most relevant subtitles.
   - Displays results with adjustable settings for better control.

## Key Features
✅ Works with large subtitle datasets efficiently.
✅ Uses **document chunking** to maintain context in long subtitles.
✅ Supports both **keyword-based** and **AI-powered semantic search**.
✅ Provides fast and accurate subtitle retrieval.
✅ Built using **Python, ChromaDB, AssemblyAI, and Streamlit**.

## Tech Stack
- **Data Processing**: Python, pandas, numpy
- **Vectorization**: TF-IDF, SentenceTransformers (BERT-based embeddings)
- **Embedding Storage**: ChromaDB
- **Audio Transcription**: AssemblyAI
- **Web App**: Streamlit

This approach ensures that video subtitles are easy to search, making content more accessible and improving user experience!
