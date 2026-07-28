# Retrieval-Augmented Generation (RAG) Based Agentic AI Chatbot

An intelligent multi-agent conversational AI system that combines Retrieval-Augmented Generation (RAG), vector search, and autonomous AI agents to provide accurate, context-aware, and explainable responses. The project leverages modern LLM frameworks to retrieve relevant information from external knowledge sources before generating responses, reducing hallucinations and improving factual accuracy.

> **CSC 583 – Natural Language Processing Final Project**
>
> **Author:** Kunal Jatin Tamhane

---

## Project Overview

Large Language Models are powerful but are limited by outdated knowledge and hallucinations. This project addresses these limitations by implementing a Retrieval-Augmented Generation (RAG) pipeline integrated with an Agentic AI architecture.

Instead of relying solely on an LLM's internal knowledge, the chatbot:

- Retrieves relevant documents from a vector database
- Uses semantic search to identify the most relevant context
- Employs autonomous AI agents to plan and execute tasks
- Generates grounded, context-aware responses
- Maintains conversational memory for follow-up questions

The system demonstrates how multiple AI components can collaborate to produce more reliable and explainable answers.

---

## Features

- Retrieval-Augmented Generation (RAG)
- Agentic AI workflow
- Semantic document search
- Vector database integration
- Conversational memory
- Multi-turn dialogue support
- Context-aware response generation
- LLM-powered reasoning
- Document ingestion pipeline
- Modular architecture for future extensions

---

## System Architecture

```
User Query
      │
      ▼
 AI Agent / Planner
      │
      ▼
Retriever
(Vector Database)
      │
Relevant Documents
      ▼
Prompt Construction
      │
      ▼
Large Language Model
      │
      ▼
Final Response
```

---

## Tech Stack

### Programming Language

- Python

### AI & NLP

- Large Language Models (LLMs)
- Retrieval-Augmented Generation (RAG)
- Embedding Models

### Frameworks

- LangChain / LangGraph (if applicable)
- Hugging Face Transformers
- OpenAI APIs

### Vector Database

- FAISS / ChromaDB (depending on implementation)

### Machine Learning Libraries

- PyTorch
- NumPy
- Pandas

### Development Environment

- Jupyter Notebook
- Google Colab
- VS Code

---

## Project Structure

```
.
├── CSC_583_NLP_Final_Project.ipynb
├── README.md
├── data/
│   ├── raw_documents/
│   └── processed_documents/
├── embeddings/
├── vector_store/
├── models/
├── outputs/
└── requirements.txt
```

> Folder names may vary depending on the implementation.

---

## Workflow

### 1. Data Collection

Documents are collected from the selected knowledge source and prepared for indexing.

---

### 2. Document Preprocessing

- Cleaning
- Chunking
- Tokenization
- Metadata generation

---

### 3. Embedding Generation

Each document chunk is converted into dense vector embeddings using an embedding model.

---

### 4. Vector Database Creation

Embeddings are stored inside a vector database for efficient semantic retrieval.

---

### 5. Query Processing

When a user submits a question:

- Query embedding is generated
- Similar documents are retrieved
- Context is assembled

---

### 6. Agent Reasoning

The AI agent:

- Determines required actions
- Retrieves additional context if needed
- Plans the response
- Passes context to the LLM

---

### 7. Response Generation

The LLM generates a grounded answer using both:

- Retrieved knowledge
- User query
- Conversation history

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Retrieval-Augemented-Generation-RAG-based-Agentic-AI-Chatbot.git

cd Retrieval-Augemented-Generation-RAG-based-Agentic-AI-Chatbot
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
CSC_583_NLP_Final_Project.ipynb
```

Run all cells sequentially.

---

## Example Usage

Example query:

```
User:
What are the major applications of Retrieval-Augmented Generation?
```

Output:

```
The system retrieves relevant documents from the knowledge base,
provides supporting context to the language model,
and generates an evidence-grounded response discussing
applications such as enterprise search,
customer support,
question answering,
and document summarization.
```

---

## Learning Outcomes

This project demonstrates practical implementation of:

- Retrieval-Augmented Generation
- Agentic AI systems
- Semantic search
- Vector databases
- Embedding models
- Prompt engineering
- LLM orchestration
- Conversational AI
- Context-aware response generation

---

## Future Improvements

- Multi-agent collaboration
- Web search integration
- Hybrid retrieval
- Knowledge graph support
- Streaming responses
- Tool calling
- Voice interface
- Citation generation
- User authentication
- Production deployment with Docker and Kubernetes

---

## Results

The project successfully demonstrates that integrating Retrieval-Augmented Generation with Agentic AI significantly improves response quality by:

- Reducing hallucinations
- Improving factual consistency
- Retrieving domain-specific knowledge
- Producing context-aware responses
- Supporting complex multi-turn conversations

---

## Acknowledgements

This project was completed as part of **CSC 583 – Natural Language Processing** at **DePaul University**.

Special thanks to the course instructors, the open-source AI community, and the developers of LangChain, Hugging Face, OpenAI, and other libraries that made this project possible.

---

## License

This project is intended for educational and research purposes.

---

## Author

**Kunal Jatin Tamhane**

- GitHub: https://github.com/kunaljtamhane
- LinkedIn: https://linkedin.com/in/kunaltamhane

---
