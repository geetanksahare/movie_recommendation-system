# 🎬 Movie Recommendation System

A Content-Based Movie Recommendation System that suggests similar movies based on user selection.  
Built using Machine Learning and deployed as an interactive web application with Streamlit.

🔗 **Live App:**  
https://movierecommendation-system-gs.streamlit.app/

---

## 📌 Project Overview

Recommender systems are widely used in platforms like Netflix and Amazon to personalize content for users.

This project implements a **content-based filtering approach** that:

- Computes similarity between movies  
- Recommends top 5 similar movies  
- Fetches real-time movie posters using TMDB API  
- Provides an interactive Streamlit interface  

The system allows users to select a movie and instantly receive recommendations.

---

## 🧠 Recommendation Approach

### 1️⃣ Data Processing

- Movie dataset preprocessing  
- Feature extraction from movie metadata  
- Creation of a similarity matrix  

---

### 2️⃣ Similarity Computation

- Content-based filtering  
- Cosine similarity matrix generation  
- Precomputed similarity stored using pickle  

When a user selects a movie:
- The system finds its index  
- Retrieves similarity scores  
- Sorts movies by similarity  
- Returns top 5 most similar titles  

---

## 🎥 Poster Fetching

Movie posters are dynamically fetched using the **TMDB API**.

- Movie ID is extracted  
- API request is sent  
- Poster path is retrieved  
- Image displayed in Streamlit  

This enhances user experience by making recommendations visually interactive.

---

## 🤖 Model & Files

- `movie_list.pkl` → Preprocessed movie dataset  
- `similarity.pkl` → Precomputed similarity matrix  
- Model artifacts auto-download during first deployment run (via Google Drive)  

---

## 🌐 Deployment

Built with:

- Streamlit  
- Requests (for API calls)  
- gdown (for downloading large similarity file)  

Users can:

- Select a movie from dropdown  
- Click “Show Recommendation”  
- View 5 recommended movies with posters  

---

## 🛠️ Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Streamlit  
- Requests  
- gdown  

(Dependencies listed in requirements file :contentReference[oaicite:0]{index=0})

Main application logic implemented in `app.py` :contentReference[oaicite:1]{index=1}

---

## 📂 Project Structure

```
movie-recommendation-system/
│
├── app.py
├── movie_recommendation.ipynb
├── movie_list.pkl
├── similarity.pkl
├── requirements.txt
└── README.md
```

---

## ⚙️ How to Run Locally

```bash
# Clone repository
git clone https://github.com/geetanksahare/movie-recommendation-system.git

# Navigate to project folder
cd movie-recommendation-system

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py
```

---

## 📊 Example Workflow

1. Select: *Inception*  
2. Click: **Show Recommendation**  
3. System displays 5 similar movies with posters  

---

## 🔥 Key Highlights

- Content-based recommendation system  
- Cosine similarity implementation  
- Precomputed similarity matrix optimization  
- Real-time poster fetching using external API  
- Interactive UI with Streamlit  
- Deployment-ready architecture  

---

## 🎯 Learning Outcomes

- Understanding recommendation system fundamentals  
- Similarity matrix computation  
- API integration in ML projects  
- Model serialization using pickle  
- Deploying ML apps using Streamlit  
