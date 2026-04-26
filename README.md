# RAG AI Project: Local Video-to-Knowledge Pipeline

This is a fully local **Retrieval-Augmented Generation (RAG)** system designed to process video content, transcribe it, and allow for intelligent querying. It uses state-of-the-art open-source models to ensure data privacy and high performance.

## 🧠 AI Stack
- **Transcription**: `OpenAI Whisper Large-v2` (High-accuracy speech-to-text)
- **Embeddings**: `BGE-M3` via Ollama (Multi-lingual, high-density vector embeddings)
- **LLM**: `Llama 3.2` via Ollama (Context-aware reasoning)
- **Processing**: `FFmpeg` for media handling

## 📁 Project Structure
- `vdo_to_mp3.py`: Extracts audio from video files using FFmpeg.
- `speech_to_text.py`: Transcribes audio into JSON using Whisper Large-v2.
- `preprocess_json.py`: Cleans and segments transcriptions for embedding.
- `mp3_to_json.py`: Direct conversion utility.
- `process_incoming.py`: Main pipeline for handling new queries.
- `prompt_template.txt`: Template used to structure LLM instructions.

## 🛠️ Prerequisites
Before running the project, ensure you have the following installed:

1. **FFmpeg**: Required for media conversion.
   ```bash
   brew install ffmpeg
