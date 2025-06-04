# 📚 Semantic Book Recommender

A smart book recommendation system that understands the **semantics** of your input. Instead of relying on traditional metadata filters (like genre or author), this system leverages **transformer-based embeddings** to find books that are *semantically similar* to your query.

## 🚀 Features

- 🔎 **Semantic Search**: Finds books based on deep language understanding, not just keyword matches.
- 🧠 **Transformer Embeddings**: Uses OpenAI embeddings via LangChain.
- 🗃️ **Vector Store**: Efficient similarity search using ChromaDB.
- 🎛️ **Interactive UI**: Built with Gradio to easily enter queries and view results.
- 📦 **Kaggle Dataset**: Uses a dataset of 7,000+ books with rich metadata and descriptions.

## 📁 Dataset

Sourced from [Kaggle](https://www.kaggle.com/datasets/dylanjcastillo/7k-books-with-metadata). Downloaded using the `kagglehub` library.

## 🧠 How It Works

1. **Load and preprocess** the book descriptions from the dataset.
2. **Generate embeddings** for book descriptions using OpenAI's models.
3. **Store vectors** in ChromaDB for fast retrieval.
4. **Take user input** through a Gradio interface.
5. **Find and display** the most similar books based on cosine similarity of embeddings.

## 💻 Installation

```bash
pip install python-dotenv langchain-community langchain-openai langchain-chroma transformers gradio kagglehub
