# Movie Recommendation System 🎬

This project recommends movies to users based on their ratings and genres using machine learning techniques.  

---

## Project Overview
The goal of this project is to provide movie recommendations by analyzing user ratings and movie metadata. The system reduces data sparsity, encodes movie genres, clusters similar movies, and provides recommendations based on cluster similarity.  

---

## Dataset
- **Movies Data:** Contains movie titles, IDs, and genres.  
- **Ratings Data:** Contains user IDs, movie IDs, and ratings.  

**Key features used:**  
- **Numerical:** Ratings  
- **Categorical:** Genres  

---

## Steps Performed

### 1. Data Loading
- Loaded movies and ratings datasets using Pandas.  

### 2. Data Cleaning
- Checked for null values and removed entries with missing data.  

### 3. Filtering Users and Movies
- **Users:** Only include users who rated more than 50 movies.  
- **Movies:** Only include movies with at least 10 ratings.  
- This step reduces sparsity in the dataset.  

### 4. One-Hot Encoding
- Converted movie genres into a one-hot encoded matrix to represent each genre as a separate binary feature.  

### 5. Clustering
- Applied the **Elbow Method** to determine the optimal number of clusters for KMeans.  
- Used **KMeans clustering** to group similar movies based on their genre features.  

### 6. Recommendation Function
- Created a function that takes a movie name as input and returns a list of similar movies from the same cluster.  

### 7. Movie Recommendations
- Tested the recommendation function with sample movies to verify meaningful results.  

---

## Tech Stack
- Python 3  
- Libraries: pandas, numpy, scikit-learn, matplotlib
