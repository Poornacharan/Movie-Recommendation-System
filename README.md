# Movie-Recommendation-System
This project is a Content-Based Recommendation System that suggests movies similar to a given movie using Natural Language Processing (NLP) techniques and cosine similarity. It analyzes movie metadata like genres, cast, crew, overview, and keywords to compute similarity scores between movies.

Key Features:
-Recommends top 5 movies based on content similarity.
-Uses text processing and stemming to normalize textual data.
-Implements cosine similarity to find similar movies.
-Includes a Streamlit-based web interface for interactive recommendations.
-Pulls movie posters from the TMDB API to enhance the UI.

Dataset Used:
-TMDB 5000 Movie Dataset (tmdb_5000_movies.csv and tmdb_5000_credits.csv)
-Includes metadata like title, overview, cast, crew, genres, and keywords.
-Joined on the title column to form a comprehensive dataset.

Tech Stack:
-Language: Python
-Libraries:pandas, numpy for data preprocessing
-ast for parsing stringified lists
-NLTK for stemming (PorterStemmer)
-scikit-learn for feature extraction (CountVectorizer) and similarity (cosine_similarity)
-requests for API calls
-Streamlit for web UI

API: TMDB API (for fetching movie posters)
