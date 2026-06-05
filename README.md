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

Unlike traditional collaborative filtering systems, the model recommends music directly from the semantic and emotional content of user prompts.

## Results

The paper evaluates both explicit and implicit emotional prompts across:
- Joy
- Sadness
- Fear
- Anger

Key findings:
- **MRR@10: 0.78**
- **nDCG@10: 0.80**
- Strong emotional alignment between prompts and retrieved songs
- **0 hallucinated recommendations** across all tested LLMs

## Example Prompt

> “The walls feel like they are closing in”

The retriever identifies lyrically relevant songs, while the generator produces a curated playlist grounded entirely in retrieved evidence.

## Motivation

This project explores how RAG systems can improve music recommendation by incorporating:
- emotional intent
- lyrical meaning
- contextual reasoning

instead of relying primarily on listening history or popularity signals.

