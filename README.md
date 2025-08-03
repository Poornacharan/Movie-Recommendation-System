🎬 Movie Recommender System
A content-based movie recommender system that suggests similar movies based on metadata like genres, keywords, cast, crew, and overview. Built with Python, NLP techniques, and deployed with a Streamlit interface. Posters are fetched dynamically using the TMDB API.

📌 Features
-Recommends top 5 movies similar to a selected movie
-Uses content features (genre, keywords, cast, crew, overview)
-Applies NLP and cosine similarity to compute relevance
-Fetches movie posters using TMDB API
-Interactive web UI using Streamlit

🧠 How It Works
Data Preprocessing:
Combined movie data (tmdb_5000_movies.csv + tmdb_5000_credits.csv)
Extracted useful fields: genres, keywords, cast, crew, overview
Removed nulls and cleaned data
Applied stemming and token normalization

Vectorization:
Used CountVectorizer (with top 5000 words and English stop words removed)
Created vectors from the final tags column

Similarity Calculation:
Calculated cosine similarity between movie vectors
Stored similarity matrix for efficient recommendations

Recommendation:
Takes a movie title and returns 5 most similar movies
Also fetches posters using the TMDB API

🖥️ Tech Stack
Python
pandas, numpy
scikit-learn
nltk
requests (for TMDB API)
Streamlit (for web interface)

📁 Files
| File / Folder           | Description                   |
| ----------------------- | ----------------------------- |
| `app.py`                | Main Streamlit app            |
| `tmdb_5000_movies.csv`  | Movie metadata                |
| `tmdb_5000_credits.csv` | Movie credits (cast, crew)    |
| `movie_dict.pkl`        | Preprocessed movie dictionary |
| `similarity.pkl`        | Precomputed similarity matrix |
| `README.md`             | Project documentation         |
