# MOVIELENS RECOMMENDATION SYSTEM
![movielens](avatar.jpg)

Overview of the project:
1. [INTRODUCTION](#introduction)
2. [BUSINESS UNDERSTANDING](#business-understanding)
3. [DATA UNDERSTANDING](#data-understanding)
4. [DATA PREPARATION](#data-preparation)
5. [EXPLORATORY DATA ANALYSIS](#exploratory-data-analysis)
6. [MODELLING](#modelling)
7. [CONCLUSION](#conclusion)
8. [RECOMMENDATIONS](#recommendations)
## Introduction
In today's world of countless movie options, it can be challenging for users to find movies that match their preferences. Recommendation systems come to the rescue by offering personalized movie recommendations based on user ratings. In this task, we aim to build a recommendation system using the MovieLens dataset to provide users with their top 5 movie recommendations.

## Business Understanding
The goal of this recommendation system is to enhance the movie-watching experience for users by suggesting movies that they are likely to enjoy based on their ratings of other movies. By offering personalized recommendations, we can increase user engagement, satisfaction, and ultimately drive user retention on the platform.

## Problem Statement
The problem is to build a recommendation system that can accurately predict and recommend the top 5 movies for a user based on their ratings of other movies. The system should leverage collaborative filtering techniques and content based filtering techniques to analyze user preferences and generate accurate recommendations.

## Metric of success
Root Mean Squared Error (RMSE): RMSE is a commonly used evaluation metric for recommendation systems that deal with explicit ratings. It measures the average magnitude of the differences between the predicted ratings and the actual ratings given by users. A lower RMSE indicates better accuracy and performance of the recommendation system.

Mean Absolute Error (MAE): MAE is another widely used metric for recommendation systems. It calculates the average absolute difference between the predicted ratings and the actual ratings. MAE provides a measure of how well the recommendation system can estimate user preferences without considering the direction of the errors. Like RMSE, a lower MAE indicates better accuracy and performance of the recommendation system.

## Data Exploration

### Data Understanding
The Data sourced for this project was the "movielens Dataset" which was sourced from grouplens.org/datasets/movielens.
The dataset includes:

`ratings.csv`: This file contains user ratings for movies. It includes the following columns:
- **userId**: The ID of the user who provided the rating.
- **movieId**: The ID of the movie being rated.
- **rating**: The rating given by the user to the movie (on a scale of 0.5 to 5 in increments of 0.5).
- **timestamp**: The timestamp when the rating was recorded.

`movies.csv`: This file contains information about movies. It includes the following columns:
- **movieId**: The ID of the movie.
- **title**: The title of the movie along with the release year.
- **genres**: The genre(s) of the movie, separated by "|" if multiple genres apply.

`tags.csv`:This file contains user-generated tags for movies.
Each row represents a specific tag assigned by a user to a movie.

`links.csv`:This file contains links to external movie databases (IMDb and TMDB).

