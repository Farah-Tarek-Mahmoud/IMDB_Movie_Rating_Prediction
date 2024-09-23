# IMDB Movie Rating Prediction Project

## Overview

This project aims to predict movie ratings based on various features from an IMDB dataset, using machine learning models like Lasso, RandomForestRegressor, GradientBoostingRegressor, and AdaBoostRegressor. The dataset contains features such as genre, director, actors, votes, year, and duration of the movies.

## Dataset

The dataset, **IMDB Movies India.csv**, includes the following columns:
- **Name**: Title of the movie
- **Genre**: Movie genre
- **Director**: Director of the movie
- **Actor 1, Actor 2, Actor 3**: Main actors
- **Year**: Release year
- **Duration**: Duration of the movie
- **Votes**: Number of votes received
- **Rating**: IMDB rating of the movie

### Data Preprocessing
1. **Handling Missing Values**: Visualized missing data using heatmaps, dropped columns with more than 5% missing values, and imputed missing values where necessary.
2. **Feature Engineering**: 
   - Extracted and cleaned data from columns like `Year`, `Votes`, and `Duration`.
   - Categorical features like `Genre`, `Director`, `Actors`, and `Name` were encoded by averaging the ratings for each category.
3. **Standardization**: Numerical features such as `Votes`, `Duration`, and `Year` were standardized using `StandardScaler`.

### Exploratory Data Analysis (EDA)
- Distribution of the `Rating` column was visualized using histograms.
- Correlations between numerical variables were explored using heatmaps.
- Popular movie genres were visualized through bar charts.

## Models Implemented

1. **Lasso Regression**: Used to evaluate the performance with regularization.
2. **Random Forest Regressor**: An ensemble method to improve prediction accuracy.
3. **Gradient Boosting Regressor**: A boosting technique applied to improve performance.
4. **AdaBoost Regressor**: Another boosting model used for experimentation.

## Model Evaluation

The models were evaluated using:
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R-Squared (R²)**

You can run the models to get the current evaluation metrics.

## Requirements
- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
