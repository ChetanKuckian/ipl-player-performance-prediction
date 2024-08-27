# Machine Learning Models for IPL Player Performance Prediction and Recommendation

## Introduction

Cricket, particularly the Indian Premier League (IPL), generates a significant amount of interest and data. This project leverages artificial intelligence to enhance player performance analysis and prediction. We have developed three machine learning models:

1. **Player Recommendation Model**: Uses clustering to recommend players with similar profiles.
2. **Batsman Performance Prediction Model**: Predicts if a batsman will score more than 30 runs in an upcoming match.
3. **Bowler Performance Prediction Model**: Predicts if a bowler will take at least one wicket in an upcoming match.

The goal is to provide teams and analysts with advanced tools for data-driven decision-making to improve strategies and performance.

## PowerPoint Presentation

For a comprehensive summary of the project, including objectives, methodologies, and results, please refer to the PowerPoint presentation available in this repository.

## Dataset

The dataset includes IPL match history from 2008 to 2023, featuring batting and bowling cards, match summaries, and points tables. This data provides a comprehensive view of player performances across various seasons and conditions.

- **[IPL Dataset (2008-2022) on Kaggle](https://www.kaggle.com/datasets/jhalls/ipl-dataset-2008-2022)**

### Data Files

- `all_season_batting_card.csv`: Contains batting information for each match.
- `all_season_bowling_card.csv`: Contains bowling information for each match.
- `all_season_summary.csv`: Contains match summaries including teams, toss results, and winners.

## Data Exploration

Exploratory data analysis includes:

- **Scatter Plots**: Examining the relationship between runs scored and balls faced.
- **Top Batsmen and Bowlers**: Identifying players with the most fours, sixes, and wickets.
- **Histograms**: Understanding the distribution of runs scored and wickets taken.
- **Box Plots**: Analyzing the distribution of wickets and runs conceded.

## Player Recommendation Using K-Means

The player recommendation system uses K-Means clustering to group players based on their performance metrics. Features for clustering include:

- **Batting Metrics**: Average runs, strike rate, etc.
- **Bowling Metrics**: Average overs, economy rate, wickets taken, etc.

Silhouette scores are used to determine the optimal number of clusters. The clusters help recommend players with similar performance profiles.

## Performance Prediction Models

### Batsman Performance Prediction

This model predicts whether a batsman will score more than 30 runs in an upcoming match. Features include:

- Team and venue information
- Recent performance metrics
- Opponent team statistics

### Bowler Performance Prediction

This model predicts whether a bowler will take at least one wicket in an upcoming match. Features are similar to those used for batsman prediction but focused on bowling metrics.

## Model Evaluation

Models are evaluated based on:

- **Accuracy**: Measures the overall performance of the model.
- **Classification Report**: Provides precision, recall, and F1-score for different classes.

## Usage

To use the models, follow these steps:

1. **Data Preparation**: Ensure that you have the necessary datasets and perform preprocessing as required.
2. **Model Training**: Use the provided features to train the models.
3. **Prediction**: Utilize the trained models to make predictions on new data.