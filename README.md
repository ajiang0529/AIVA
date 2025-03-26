# HWVA - Homework Virtual Assistant

## Project Overview
HWVA (Homework Virtual Assistant) is a lightweight chatbot application that leverages OpenAI's GPT models to provide intelligent responses based on user-provided training documents. It uses a vector index to search and respond with context-aware answers. The interface is built using Gradio for ease of use.

## Features
- Document-based knowledge retrieval
- Gradio web interface for easy interaction
- Configurable AI model using GPT-3.5 Turbo
- Simple directory-based document loading

## Prerequisites
- Python 3.7+
- OpenAI API Key

## Installation

### Dependencies
```bash
pip install gpt_index langchain gradio openai
```

### Setup
1. Clone the repository
2. Set your OpenAI API key in the script
3. Place training documents in the `trainingDocs` directory

## Configuration
- Adjust model parameters in `construct_index()`:
  - `max_input_size`: Maximum input token size
  - `num_outputs`: Maximum response token size
  - `temperature`: Controls response randomness

## Usage
```bash
python AIVA.py
```
The script will:
- Index documents from `trainingDocs`
- Launch a Gradio web interface
- Allow interactive querying of your document collection

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
