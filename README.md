# AIVA - AI Virtual Assistant

## Project Overview
AIVA is an AI-powered chatbot that uses document indexing and retrieval to provide intelligent responses based on a collection of training documents.

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

## Security Note
⚠️ **Important**: Remove or replace the OpenAI API key before sharing the project publicly.

## License
[Add your project's license here]

## Contributing
[Add contribution guidelines if applicable]
