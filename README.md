# Music-Popularity-Prediction
This project implements a machine learning–based approach to predict music popularity using audio and metadata features.

# 🎵 Music Popularity Prediction

This project analyzes Spotify music data to determine which audio features contribute most to a track's popularity.
It implements a Machine Learning pipeline using a **Random Forest Regressor** 
to predict popularity scores based on features like energy, danceability, and loudness.

## 📌 Project Overview
The goal of this project is to understand the drivers of music popularity and build a predictive model.
By analyzing acoustic characteristics, we can identify patterns that make a song successful on streaming platforms.

## 📂 Dataset
The project uses a dataset (`Spotify_data.csv`) containing various audio features for tracks.
* **Target Variable**: `Popularity` (Numeric score)
* **Key Features**:
  * `Energy`, `Valence`, `Danceability`
  * `Loudness`, `Acousticness`, `Tempo`
  * `Speechiness`, `Liveness`

## ⚙️ Methodology

1.  **Data Cleaning**: Removal of unnecessary columns (e.g., `Unnamed: 0`) to prepare the dataset.
2.  **Exploratory Data Analysis (EDA)**:
    * **Correlation Analysis**: Identified that `Loudness` and `Danceability` have a moderate positive correlation with popularity, while `Acousticness` shows a negative correlation.
    * **Visualizations**: Uses scatter plots and histograms to visualize feature distributions and relationships.
3.  **Preprocessing**:
    * Data splitting into training and testing sets.
    * Feature scaling using `StandardScaler` to normalize the data.
4.  **Model Training**:
    * **Algorithm**: Random Forest Regressor.
    * **Hyperparameter Tuning**: Utilizes `GridSearchCV` to optimize parameters like `n_estimators`, `max_depth`, and `min_samples_split`.

## 📊 Results
* The Random Forest model was selected for its superior performance compared to other baseline algorithms.
* **Evaluation**: The model's predictions were visualized against actual popularity scores, showing a strong clustering around the "perfect prediction" line, indicating high accuracy.

## 🛠️ Installation & Usage

### Prerequisites
* Python 3.x
* Jupyter Notebook

Running the Project
Clone this repository.

Ensure Spotify_data.csv is in the project directory.
Open the notebook:

jupyter notebook Music_Popularity_Prediction_.ipynb
Run all cells to execute the analysis and training pipeline.
### Required Libraries
Install the necessary Python packages:
```bash

pip install pandas numpy matplotlib seaborn scikit-learn
Author
Abhijeet Patange


