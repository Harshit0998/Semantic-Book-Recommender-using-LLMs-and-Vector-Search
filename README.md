This project builds an intelligent semantic book recommendation system using LLMs, embeddings, vector databases, and emotion analysis.
Instead of keyword search, users can query in natural language like:

“A story about revenge and betrayal”
“A joyful non-fiction book about personal growth”

and receive highly relevant book recommendations filtered by category and emotional tone.

The system combines text cleaning, vector search, zero-shot classification, sentiment analysis, and a Gradio web app into a complete end-to-end ML application.

Features
 Text data cleaning and preprocessing of book descriptions
 Semantic (vector) search using OpenAI embeddings and ChromaDB
 Zero-shot classification to label books as Fiction / Non-Fiction
 Emotion & sentiment extraction from descriptions (joy, fear, anger, sadness, surprise)
 Interactive Gradio dashboard for real-time recommendations
 Project Structure
File	Description
data-exploration.ipynb	Text cleaning, preprocessing, and dataset preparation
vector-search.ipynb	Creating embeddings and building the Chroma vector database
text-classification.ipynb	Zero-shot classification using LLMs
sentiment-analysis.ipynb	Emotion extraction and sentiment scoring using LLMs
gradio-dashboard.py	Web app for semantic book recommendations
 How It Works
Book descriptions are cleaned and processed.
OpenAI embeddings are created for each book description.
Embeddings are stored in a Chroma vector database.
Users enter a natural language query.
The system performs semantic similarity search.
Results are filtered by:
Category (Fiction / Non-Fiction)
Emotional tone (Happy, Suspenseful, Sad, Angry, Surprising)
Results are displayed in a Gradio dashboard with book covers and summaries.
 Tech Stack
Python 3.11
Pandas, Matplotlib, Seaborn
LangChain
OpenAI Embeddings
ChromaDB (Vector Database)
Transformers (Zero-shot classification)
Gradio (Web UI)
 Setup Instructions
1️⃣ Clone the repository
git clone <your-repo-link>
cd <repo-name>
2️⃣ Install dependencies
pip install -r requirements.txt
3️⃣ Add OpenAI API key

Create a .env file in the root directory:

OPENAI_API_KEY=your_key_here
4️⃣ Download dataset from Kaggle

Follow the instructions in the notebooks to download and prepare the dataset using kagglehub.

5️⃣ Build the vector database

Run:

data-exploration.ipynb
vector-search.ipynb
text-classification.ipynb
sentiment-analysis.ipynb
6️⃣ Launch the web app
python gradio-dashboard.py
 Example Queries
“A suspenseful mystery involving a detective”
“A happy non-fiction book about success”
“A sad story about war and loss”
“A surprising sci-fi adventure”
 Learning Outcomes

This project demonstrates practical use of:

Embeddings & vector similarity search
LLM zero-shot classification
Emotion mining from text
Building end-to-end AI applications
Deploying ML systems with user interfaces
