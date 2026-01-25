# 🎬 Movie Recommendation System

A content-based movie recommendation system using **TF-IDF vectorization** and **cosine similarity**, powered by a **FastAPI backend** and a **Streamlit frontend**.

---

##  Overview

This project recommends movies similar to a user-selected movie based on textual features such as overview and metadata.  
It demonstrates the complete machine learning pipeline from data preprocessing to deployment-ready(future plans) APIs and UI.

---

## Features

- Content-based movie recommendations  
- TF-IDF + cosine similarity  
- FastAPI backend with REST APIs  
- Streamlit frontend with modern UI  
- Movie posters & metadata via TMDB API   
- Genre-based recommendations  

---

## Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- FastAPI  
- Streamlit  
- TMDB API  
- Jupyter Notebook (Google Colab)

---

## Dataset

The dataset used in this project is **not included in the repository** due to size constraints.

- **Dataset name:** Movies Metadata  
- **Source:** Kaggle  (Movies dataset)
- **Link:** https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset  

To run the project locally, download `movies_metadata.csv` from Kaggle and place it inside the `data/` directory.
 
- **Used for:**  
  - Movie titles  
  - Overviews  
  - Genres and metadata  
  - Similarity computation  

---

## How It Works

1. Movie metadata is cleaned and processed in a Jupyter Notebook.
2. Textual features are converted into vectors using TF-IDF.
3. Cosine similarity is computed between movies.
4. Trained objects are saved as pickle files.
5. FastAPI loads these files and exposes recommendation endpoints.
6. Streamlit consumes the APIs and displays recommendations.

---

## Running the Project Locally

### Backend
cd backend
pip install -r requirements.txt
uvicorn main:app --reload

### Frontend
cd frontend
streamlit run app.py

## Setting up Environment Variables
TMDB_API_KEY=your_api_key_here






