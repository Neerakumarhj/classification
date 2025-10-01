# 🎵 Spotify Genre Classification

## 📌 Project Overview
This repository contains my work for the **CS985/6 Spotify Classification Problem 2025**.  
The goal is to build a machine learning model that predicts the **genre of a song** (`top genre`) from its musical attributes.

- **Type**: Multi-class classification  
- **Target**: `top genre`  
- **Features**: 13 numerical song features (e.g., bpm, energy, danceability)  
- **Evaluation Metric**: Accuracy  
- **Output**: CSV file with `Id` and predicted `top genre`  

The dataset is a slightly modified version of [Spotify Past Decades Songs 50s–10s](https://www.kaggle.com/cnic92/spotify-past-decades-songs-50s10s):  
- Column `Number` renamed to `Id`  
- Column `top genre` moved to the last position  

---

## ⚙️ Workflow
1. **Data Loading** – Imported training and test datasets.  
2. **Data Cleaning** – Removed irrelevant columns, handled missing values.  
3. **Encoding** – Encoded `top genre` labels into numbers.  
4. **EDA** – Genre distribution and correlation heatmap.  
5. **Model Training** – Used **LightGBM** classifier.  
6. **Evaluation** – Checked validation accuracy and simple observations.  
7. **Final Submission** – Trained on all data and saved predictions to `spotify_submission.csv`.  

---

## 📊 Results
- The model achieved a reasonable validation accuracy.  
- Rare genres are harder to predict due to class imbalance.  
- Final predictions are in:

