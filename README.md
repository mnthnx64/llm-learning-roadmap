# LLM Learning Workspace

This workspace is dedicated to learning about Large Language Models (LLMs) and related technologies.

## Structure

This repository is organized by learning topics:

- **nlp-foundation/**: Fundamentals of Natural Language Processing
  - `regex/`: Regular expressions for text processing
  - `text-preprocessing/`: Tokenization, stemming, lemmatization, NER, POS
  - `text-presentation/`: Count vectorizer, TF-IDF, BOW, Word2Vec, Embeddings
  - `text-classification/`: Naïve Bayes classification

- **gen-ai-fundamentals/**: Generative AI fundamentals
  - `llms-embeddings/`: Large Language Models and Embeddings
  - `vector-dbs/`: Vector Databases (FAISS, Chromadb)
  - `rag/`: Retrieval Augmented Generation
  - `langchain/`: Langchain Framework

- **project-1/**: Real-world projects
  - `real-world-projects/`: Projects using LLMs, RAG, Agents to solve real-life problems

- **agentic-ai-fundamentals/**: Agentic AI concepts
  - `what-is-agentic-ai/`: Understanding Agentic AI
  - `gen-ai-vs-agents/`: Gen AI vs AI Agents vs Agentic AI
  - `mcp/`: Model Context Protocol (MCP)

- **frameworks/**: AI agent frameworks
  - `agno/`: Building agents with Agno framework
  - `langgraph/`: Building stateful agents with LangGraph
  - `crew-ai/`: Crew AI framework
  - `google-adk/`: Google Agent Development Kit
  - `openai-adk/`: OpenAI Agent Development Kit
  - `langsmith/`: Tracing and monitoring with LangSmith

## Setup

### Prerequisites

- **Python 3.8+** (Python 3.9 or higher recommended)
- **pip** (Python package installer)
- **Virtual environment** (optional but recommended): `venv`, `conda`, or `mamba`

### Quick Start

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone <repository-url>
   cd llm-stuff
   ```

2. **Create and activate a virtual environment** (choose one option):

   **Option A: Using venv (recommended for beginners)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On macOS/Linux
   # OR
   venv\Scripts\activate  # On Windows
   ```

   **Option B: Using conda/mamba**
   ```bash
   conda create -n llm-learning python=3.9
   conda activate llm-learning
   # OR
   mamba create -n llm-learning python=3.9
   mamba activate llm-learning
   ```

3. **Install all dependencies** with a single command:
   ```bash
   pip install -r requirements.txt
   ```

4. **Download additional NLP models** (required for some notebooks):
   ```bash
   # Download spaCy English model
   python -m spacy download en_core_web_sm
   
   # Download NLTK data (run this in Python or a notebook)
   python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords'); nltk.download('averaged_perceptron_tagger'); nltk.download('wordnet')"
   ```

5. **Verify installation**:
   ```bash
   python -c "import numpy, pandas, sklearn, nltk, spacy, sentence_transformers, faiss, chromadb; print('All packages installed successfully!')"
   ```

### Running Notebooks

- Open Jupyter Notebook or JupyterLab:
  ```bash
  jupyter notebook
  # OR
  jupyter lab
  ```

- Navigate to the topic folder you want to explore (e.g., `nlp-foundation/text-preprocessing/`)

### Troubleshooting

- **Import errors**: Make sure your virtual environment is activated
- **spaCy model errors**: Run `python -m spacy download en_core_web_sm`
- **NLTK data errors**: Run the NLTK download command in step 4
- **FAISS installation issues**: If `faiss-cpu` fails, try `pip install faiss-cpu --no-cache-dir`

## Roadmap

See [roadmap.md](./roadmap.md) for the complete learning roadmap.

