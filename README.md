# Semantic Book Recommendation System

## 📌 Project Overview

This project is a **Semantic Book Recommendation System** that suggests books based on user queries by leveraging **large language models (LLMs)**. It utilizes **semantic search with a drop-down menu (category and tone) to provide relevant book recommendations.**

## 🔍 Features

- **Semantic Search**: Uses **Google Generative AI API**, implemented using the **LangChain** framework, to generate embeddings for book metadata.
- **Zero-Shot Classification**: Implements **Facebook/bart-large-mnli** from **Hugging Face** to classify books into **fiction and non-fiction** categories without fine-tuning.
- **Vector Search**: Employs **FAISS**, implemented using **LangChain**, for efficient similarity search and retrieval.
- **Sentiment Analysis Using LLMs**: Uses **j-hartmann/emotion-english-distilroberta-base** to extract emotions from book descriptions and user queries. This allows users to sort books by their tone, such as how suspenseful, joyful, or sad the books are.
- **Interactive Dashboard**: Built with **Gradio** for easy interaction with the recommendation system.

## 📂 Dataset

The project uses the **"7K Books with Metadata"** dataset from **Kaggle** ([dylanjcastillo/7k-books-with-metadata](https://www.kaggle.com/dylanjcastillo/7k-books-with-metadata)). The dataset contains information such as book titles, authors, descriptions, categories, rating, thumbnail, and more.T

## 🛠️ Tech Stack

- **Python** (Data processing, ML models)
- **LangChain** (Framework for AI pipeline)
- **Google Generative AI API** (Embedding generation via LangChain)
- **Hugging Face Models** (Zero-shot classification & sentiment analysis)
- **FAISS** (Vector database for efficient retrieval via LangChain)
- **Gradio** (Dashboard for user interaction)

## 🚀 How to Run

1. **Create a Python Virtual Environment**:

   ```bash
   python -m venv book_recommender_env
   ```
     - On Mac:
       ```bash
       source book_recommender_env/bin/activate
       ```
     - On Windows:
       ```bash
       book_recommender_env\Scripts\activate
       ```

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Gradio interface**:

   ```bash
   python gradio-dashboard.py
   ```

4. **Access the dashboard** in your browser.

## 📜 Acknowledgments

- **Kaggle** for the dataset.
- **Hugging Face** for pre-trained LLM models.
- **Google Generative AI API** for embeddings.
- **FAISS** for efficient similarity search.
- **LangChain** for streamlining the AI workflow.
- **Gradio** for an easy-to-use UI.



