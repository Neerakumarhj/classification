# 🎵 Spotify Genre Classification

This repo has my coursework for the **CS985/6 Spotify Classification Problem 2025**.  
The task was to build a model that predicts the **genre of a song** based on its features like bpm, energy, danceability and so on.  

The dataset is a modified version of a Spotify dataset from Kaggle. The only changes were:  
- `Number` column renamed to `Id`  
- `top genre` column moved to the end  

---

## What I did
- Cleaned the data (removed Id/title/artist, handled missing values)  
- Did some quick EDA (genre counts, feature correlations)  
- Encoded the target labels into numbers  
- Trained a LightGBM model with a simple train/validation split  
- Finally, trained on the whole dataset and created predictions for the test set  

---

## Output
The final predictions are saved in **spotify_submission.csv** with this format:

```csv
Id,top genre
123,rock
456,pop
789,disco
