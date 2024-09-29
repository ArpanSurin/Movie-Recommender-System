# 🎥 Movie Recommender System
This is a Movie Recommender System built using Streamlit and The Movie Database (TMDB) API.\
It provides movie recommendations based on similarity scores between movies, and it fetches and displays movie posters from the TMDB API.

[Dataset Link](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## 🔍 Project Overview
The Movie Recommender System recommends similar movies based on user input. The system:

- Takes a movie name as input from the user.
- Recommends 5 similar movies based on cosine similarity of movie features.
- Fetches the movie posters using the TMDB API.
- Displays the recommendations with their posters in an interactive and visually appealing format.

## 🎯 Features
- **Movie Similarity :** Recommends movies based on feature similarity.
- **Interactive UI :** Built using Streamlit for a smooth, user-friendly experience.
- **API Integration :** Uses TMDb API to fetch movie posters dynamically.
**Poster Display :** Presents the recommendations along with their posters.

## 🛠️ Technologies Used
- **Python :** Core language for developing the recommender system.
- **Streamlit :** A fast way to build and share web applications with the Python community.
- **Pandas :** For data manipulation and loading the movie dataset.
- **Pickle :** For loading precomputed similarity scores and movie metadata.
- **Requests :** For making HTTP requests to the TMDb API.
- **TMDB API :** To fetch movie posters and details.

## 📦 Installation
To set up the project locally, follow these steps:
1. **Clone the repository :**
```bash
git clone https://github.com/ArpanSurin/Movie-Recommender-System.git
cd Movie-Recommender-System
```

2. **Create a virtual environment (optional but recommended) :**
```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

3. **Install the required dependencies :**
```bash
pip install -r requirements.txt
```

4. **Get your TMDB API Key :**

- Sign up on The Movie Database (TMDB) to get an API key.
- Replace the placeholder `api_key` in the code with your API key.
Run the Streamlit app:

```bash
streamlit run app.py
```

## 🖥️ Usage
- **Input Movie Name :** Select a movie from the dropdown list.
- **Get Recommendations :** Click on the `Recommend` button.
- **View Results :** See 5 recommended movies along with their posters.

## ⚙️ How It Works
1. **Movie Data :** The movies dataset is preloaded and contains metadata like movie titles and IDs.
2. **Cosine Similarity :** A precomputed matrix of movie similarities is stored in a pickle file.
3. **Recommendation Engine :** When a user selects a movie, the app retrieves similar movies by calculating cosine similarities.
4. **API Calls :** For each recommended movie, the TMDb API fetches the corresponding movie poster.
5. **Display :** The recommended movie titles and posters are displayed in a grid.

## 👏 Acknowledgments
Special thanks to **TMDB** for providing the API and movie data.