# Movie-Recommender-System
A Streamlit-based web application that recommends movies based on genre similarity using TF-IDF and cosine similarity.

📌 Overview

This project is a content-based movie recommender system built using:

Python

Pandas

Scikit-learn (TF-IDF)

Streamlit

Cosine Similarity

Users select a movie and receive a list of similar movies based on shared genres.
The app runs in the browser and requires no installation beyond running one command.

🎯 Features

✔ Genre-based movie recommendations
✔ Clean Streamlit UI
✔ Fast TF-IDF vectorization
✔ Lightweight — works with minimal data
✔ Supports any dataset containing title and genres

📁 Dataset

Your dataset contains the following columns:

Column	Description
movieId	Unique identifier for each movie
title	Movie title
genres	Genres separated by `

Example:

movieId | title                         | genres
1       | Toy Story (1995)              | Adventure|Animation|Children|Comedy|Fantasy
2       | Jumanji (1995)                | Adventure|Children|Fantasy
3       | Grumpier Old Men (1995)       | Comedy|Romance

🧠 How It Works

Genres are transformed into TF-IDF vectors

Similarity between movies is calculated using cosine similarity

The app finds the most similar movies to the selected title

Recommendations are displayed instantly on the UI

🚀 Installation & Usage
1. Clone the repository
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender

2. Install dependencies
pip install -r requirements.txt

3. Run the Streamlit app
streamlit run app.py

🧩 Project Structure
📁 movie-recommender/
│── app.py
│── movies.csv
│── requirements.txt
│── README.md

🖥️ Streamlit App Preview

What the app does:

Displays a dropdown of all movie titles

Computes similarity scores

Shows the top recommended movies

Displays genres for each recommendation

🧪 Example Code Snippet
tfidf = TfidfVectorizer(token_pattern=r"(?u)\b\w+\b")
tfidf_matrix = tfidf.fit_transform(movies['genres'])
cosine_sim = linear_kernel(tfidf_matrix, tfidf_matrix)

📦 Requirements
streamlit
pandas
scikit-learn

You’ve hit the Free plan limit for GPT-5.
You need GPT-5 to continue this chat because there's an attachment. You
