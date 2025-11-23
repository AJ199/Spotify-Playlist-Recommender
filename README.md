# Audio-Based Songs for Personalized Playlist Recommendations on Spotify

This project explores how **Spotify audio features** can be used to build machine learning models that predict song characteristics, group similar tracks, and classify songs based on instrumentalness.  
It uses **Python**, **pandas**, **scikit-learn**, and **visualization libraries**, with each workflow implemented as a clean Python script.

---

## Dataset

**Source:** Spotify audio dataset (1960–2019)  
Includes features such as danceability, energy, loudness, valence, instrumentalness, tempo, speechiness, and more.

---

## Tech Stack

- Python  
- NumPy  
- pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

---

## Project Overview

### **1. Regression — Predict Danceability**
Predict the *danceability* of a song using features like:
- energy  
- loudness  
- speechiness  
- acousticness  
- instrumentalness  
- valence  

**Best model:** Random Forest Regressor (R² ≈ 0.48)

---

### **2. Clustering — Group Songs by Vibe**
Unsupervised clustering is used to discover natural groups of songs based on audio patterns like energy and loudness.

Methods tested:
- K-Means  
- Mini-Batch K-Means  
- Mean Shift  
- Agglomerative Clustering  

**Best clustering:** Agglomerative — clean, meaningful clusters.

---

### **3. Classification — Predict Instrumentalness Levels**
Classify songs into:
- Low  
- Medium  
- High instrumentalness  

Models tested:
- Logistic Regression  
- Decision Tree  
- SVM  
- MLP Neural Network  

**Best model:** MLP Neural Network (~72% accuracy)

---

## Key Findings

- Neural Networks outperform classical models for classification  
- Agglomerative clustering yields the most meaningful groupings  
- Danceability prediction requires more complex feature relationships  
- Feature scaling and class imbalance handling significantly improve performance
