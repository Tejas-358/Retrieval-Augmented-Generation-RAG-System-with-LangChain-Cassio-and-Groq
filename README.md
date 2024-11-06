# Retrieval-Augmented Generation (RAG) System with LangChain, Cassio, and Groq

This project implements a **Retrieval-Augmented Generation (RAG)** system that routes user queries to either a Wikipedia search or a vectorstore based on natural language processing-related topics. The system leverages **LangChain**, **Cassio**, and **Groq** to power a question-routing mechanism, embedding document retrieval, and AI-powered response generation.

## Overview
The RAG system is designed to dynamically route user questions to the most relevant data source. It uses a combination of Wikipedia search for general queries and a pre-trained vectorstore for specialized queries related to **Natural Language Processing (NLP)**, **Retrieval-Augmented Generation (RAG)**, and **LangChain**. The system works as follows:

1. **Question Routing:** Routes questions to either a Wikipedia search or a vectorstore based on the topic.
2. **Document Retrieval:** Retrieves relevant documents from the vectorstore or performs a web search using Wikipedia's API.
3. **AI-powered Response Generation:** Generates answers using Groq and other language models (LLMs).
4. **Graph-based Workflows:** The entire system is designed with LangChain’s graph-based workflow, ensuring modularity and scalability.

## Features
- **Dynamic Query Routing:** Automatically decides whether to route a query to Wikipedia or vectorstore.
- **NLP and RAG Integration:** Uses LangChain to work with document loaders and embeddings to support advanced NLP topics.
- **Groq API Integration:** Leverages the Groq API to provide fast and accurate LLM-based query responses.
- **Graph Workflows:** Implements LangChain’s `StateGraph` for seamless transitions between nodes.

## Tech Stack
- **LangChain** - For building the question-routing and retrieval pipeline.
- **Cassio** - For connecting to the Astra Database and storing vector embeddings.
- **Groq** - For providing AI-powered query response generation.
- **Wikipedia API** - For general knowledge queries.
- **HuggingFace Embeddings** - For document embeddings and similarity search.
- **LangGraph** - For building graph-based workflows.

## Installation

To install and run the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/rag-system.git
   cd rag-system

2. Install the required dependencies:
  ```bash
     pip install langchain langgraph cassio langchain_community tiktoken langchain-groq langchainhub chromadb langchain_huggingface
  ```

3. Set up environment variables (e.g., Astra DB token):
   ```bash
   export ASTRA_DB_TOKEN="your_token_here"
   export ASTRA_DB_ID="your_database_id_here"
   export GROQ_API_KEY="your_groq_api_key_here"


# Example Input:
```bash
inputs = {
    "question": "What is RAG?"
}

 
