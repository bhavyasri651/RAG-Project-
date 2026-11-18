# RAG PDF Chatbot

A command-line PDF chatbot that uses Retrieval-Augmented Generation (RAG) to answer questions from a PDF document.

## Features

- Extract text from PDF files
- Split PDF text into searchable chunks
- Generate embeddings with Sentence Transformers
- Store and retrieve document chunks with ChromaDB
- Generate answers through OpenRouter
- Interactive question-and-answer loop

## Project Structure

- `app.py` - Main chatbot application
- `utils/` - PDF reading, chunking, embeddings, retrieval, and prompt utilities
- `data/` - PDF source files
- `config.py` - OpenRouter and embedding configuration
- `requirements.txt` - Python dependencies

## Setup

1. Create and activate a virtual environment.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root:

   ```env
   OPENROUTER_API_KEY=your_api_key_here
   ```

4. Place the PDF you want to use at `data/sample.pdf`.

## Run

```bash
python app.py
```

Enter a question at the prompt. Type `exit` to close the chatbot.