# Semantic Book Recommendation System Using LLMs – Project Overview

This project walks through building a smart book recommendation system powered by Large Language Models (LLMs). It’s inspired by the concepts covered in a course hosted by freeCodeCamp, but this version is described in my own words and setup.

The project breaks down into five key parts:

### 🧹 1. Preprocessing and Cleaning Book Data  
Handled in the `data-exploration.ipynb` notebook, this step involves exploring and cleaning up the book dataset so it’s ready for analysis.

### 🧠 2. Semantic Search with Vectors  
Using `vector-search.ipynb`, we build a vector database to enable semantic querying. This means users can type something like *"a story about revenge"* and get meaningful book recommendations based on content similarity.

### 🏷️ 3. Zero-Shot Text Classification  
In `text-classification.ipynb`, we use zero-shot capabilities of LLMs to tag books as either "fiction" or "non-fiction", creating a simple filter system for users.

### 😄 4. Sentiment & Emotion Analysis  
The `sentiment-analysis.ipynb` notebook dives into analyzing the emotional tone of books—whether they’re suspenseful, joyful, melancholic, etc.—to help users pick a book that fits their mood.

### 💻 5. Web-Based Recommender Dashboard  
Finally, we wrap everything into a user-friendly Gradio app using `gradio-dashboard.py`, where users can enter queries and get book suggestions in real-time.

---

## 🛠️ Tech Stack & Setup

The system was built with Python 3.11. You’ll need the following libraries to get everything running:

- `kagglehub`
- `pandas`, `matplotlib`, `seaborn` for data handling and visualization
- `python-dotenv` for managing environment variables
- Various `langchain` extensions for working with vector stores and models
- `transformers` for LLM functionality
- `gradio` for creating the interactive web interface
- `notebook` and `ipywidgets` to enable smooth Jupyter usage

All of these are listed in the provided `requirements.txt` file for easy installation.

---

## 🔐 Configuration & Data

- **API Key Setup**: You’ll need to create a `.env` file in the root folder with your OpenAI API key for the vector search and LLM components to function.
- **Dataset Access**: The book data comes from Kaggle. Instructions for downloading and using the dataset are available in the repo.
