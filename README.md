# AIVA - AI Virtual Assistant for Homework

AIVA (AI Virtual Assistant) is a simple homework bot designed to help users interact with documents and retrieve relevant information using natural language queries. It uses OpenAI's GPT models and a vector index-based search for efficient document understanding and response generation.

## Features

- Upload a directory of training documents
- Automatically indexes document content for fast query responses
- Accepts natural language questions
- Provides context-aware answers
- Interactive web interface via Gradio

## Tech Stack

- Python
- OpenAI GPT (via `langchain` and `gpt_index`)
- Gradio (for the user interface)
- GPTSimpleVectorIndex for document indexing and querying

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/aiva-homework-bot.git
cd aiva-homework-bot
