# 🎬 Movie Recommendation System

## 📌 Project Overview

This project implements a **Content-Based Movie Recommendation System** using **Machine Learning and Natural Language Processing (NLP)**.

The system recommends movies similar to a selected movie based on **genres, keywords, overview, cast, and crew information**.

A **Streamlit web application** allows users to interact with the recommender system through a simple interface.

---

# 🚀 Features

* Movie similarity detection
* Content-based recommendation
* NLP-based feature extraction
* Cosine similarity calculation
* Interactive web interface using Streamlit

---

# 🧠 Machine Learning Pipeline

Dataset
↓
Data Cleaning
↓
Feature Engineering
↓
Text Vectorization
↓
Cosine Similarity
↓
Recommendation Function
↓
Streamlit Web App

---

# 📊 Dataset

Dataset used:

**TMDB 5000 Movie Dataset**

Files:

* tmdb_5000_movies.csv
* tmdb_5000_credits.csv

These datasets contain movie metadata including:

* genres
* overview
* keywords
* cast
* crew

---

# ⚙️ Technologies Used

Python
Pandas
Scikit-Learn
Numpy
Streamlit

---

# 🧩 Core ML Concepts Used

## 1️⃣ Feature Engineering

Movie attributes are combined into a **tags column**.

Example:

Action Superhero Marvel RobertDowneyJr

This helps represent each movie as a textual description.

---

## 2️⃣ Vectorization

Text data is converted into numeric vectors using:

CountVectorizer

Example:

"action hero marvel" → [1,0,2,1]

This enables mathematical comparison between movies.

---

## 3️⃣ Cosine Similarity

Cosine similarity measures how similar two movies are.

Formula:

Cosine Similarity = cos(angle between vectors)

Values range from:

1 → identical
0 → unrelated

This allows the system to recommend movies with similar content.

---

# 📈 Recommendation Algorithm

Steps:

1. Select a movie
2. Find its index in the dataset
3. Retrieve similarity scores
4. Sort movies based on similarity
5. Return top 5 similar movies

---

# 🖥️ Web Application

The recommender system is deployed using **Streamlit**.

Users can:

1. Select a movie
2. Click "Recommend"
3. View recommended movies

Run locally using:

python -m streamlit run app.py

---

# 📂 Project Structure

movie-recommender-system

data/
 tmdb_5000_movies.csv
 tmdb_5000_credits.csv

notebook/
 recommender.ipynb

app.py
movies.pkl
similarity.pkl

README.md

---

# 🔮 Future Improvements

* Display movie posters
* Integrate TMDB API
* Use TF-IDF instead of CountVectorizer
* Implement collaborative filtering
* Deploy online using Streamlit Cloud

---

# 👨‍💻 Author

Hari
B.Tech AIML Student

This project was built as part of learning **Machine Learning and Recommendation Systems**.

**Run the notebook first to generate:**

movies.pkl
similarity.pkl