# Soundtrack 2 My Mood

*Soundtrack 2 My Mood* is a Retrieval-Augmented Generation (RAG) system for emotion-aware music recommendation.

The project introduces a new multimodal dataset of **220k+ songs** built from:
- Spotify metadata
- Genius lyrics and annotations
- ReccoBeats audio features

The system retrieves emotionally aligned songs from lyric embeddings and uses an LLM to generate grounded playlist recommendations with short contextual explanations.

## Overview
The recommendation pipeline combines:
- **BGE-M3 embeddings** for semantic lyric retrieval
- **FAISS** vector search
- **LangChain** orchestration
- Open-source LLMs including **Llama 3**, **Mistral**, and **Qwen**


