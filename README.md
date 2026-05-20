# 📚 Semantic Book Recommendation System using NLP and LLMs

This project builds a smart book recommendation system where users can search for books using **natural language queries** like:

> “A sad story about war”  
> “A happy non-fiction book about success”

Instead of keyword search, the system understands the **meaning** of the query and recommends relevant books. Users can also filter books by **category** (Fiction / Non-Fiction) and **emotional tone** (happy, sad, suspenseful, angry, surprising).

The project combines **text preprocessing**, **vector search**, **zero-shot classification**, **sentiment analysis**, and a **Gradio web application** into a complete end-to-end NLP system.

---

## 🚀 Features

- Text cleaning and preprocessing of book descriptions
- Semantic search using embeddings and a vector database (ChromaDB)
- Zero-shot classification of books as Fiction / Non-Fiction
- Emotion and sentiment extraction from descriptions
- Interactive Gradio dashboard for real-time book recommendations

---

## 🗂️ Project Structure

| File | Description |
|------|-------------|
| `data-exploration.ipynb` | Text cleaning, preprocessing, and dataset preparation |
| `vector-search.ipynb` | Creating embeddings and building the vector database |
| `text-classification.ipynb` | Zero-shot classification using LLMs |
| `sentiment-analysis.ipynb` | Emotion extraction and sentiment scoring |
| `gradio-dashboard.py` | Web app for book recommendations |

---

## 🧠 How It Works

1. Book descriptions are cleaned and processed.
2. Text is converted into embeddings using OpenAI models.
3. Embeddings are stored in a Chroma vector database.
4. User enters a natural language query.
5. Semantic similarity search retrieves relevant books.
6. Results are filtered by category and emotional tone.
7. Recommendations are displayed in a Gradio dashboard with book covers and summaries.

---

## 🛠️ Tech Stack

- Python 3.11
- Pandas, Matplotlib, Seaborn
- LangChain
- OpenAI Embeddings
- ChromaDB (Vector Database)
- Transformers (Zero-shot classification)
- Gradio (Web UI)

---
