# AndRoTate

A local-first RAG (Retrieval-Augmented Generation) application for indexing and querying markdown files, built using LangChain and FAISS.

## Overview

AndRoTate helps you interact with your markdown notes through natural language queries. It loads, indexes, and enables semantic search of your .md files, with responses enhanced by LLM context.

## Features

- **Local-First**: All data remains on your device
- **Document Processing**: Loads and chunks markdown files from your local directory
- **Vector Search**: Uses FAISS for efficient semantic retrieval
- **Conversational Interface**: Query your documents through a chat interface
- **Memory**: Maintains conversation context during sessions
- **Text-to-Speech**: Optional audio output for responses

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/AndRoTate.git
cd AndRoTate

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
# source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

## Usage

1. Place your markdown files in the `data/md-notes` directory
2. Run the indexing process to embed your documents
3. Query your documents through the provided interface

## Project Structure

```
AndRoTate/
├── data/
│   ├── md-notes/      # Place your markdown files here
│   └── vectorstore/   # Generated vector index storage
├── notebooks/         # Jupyter notebooks for development
├── requirements.txt   # Project dependencies
└── README.md          # This file
```

## Development

- Notebooks in the `notebooks/` directory demonstrate the step-by-step development process
- `01_load_and_embed.ipynb`: Document loading and embedding process

## License

[MIT License](LICENSE)
