# MovieLens Recommendation System

Authors: Samuel Robins, Jon McCaffrey

# Contents

### 1. [Overview](#overview)
### 2. [Business and Data Understanding](#bidness)
### 3. [Data Preparation](#dataprep)
### 4. [Modeling](#modeling)
### 5. [Final Model Evaluation](#final)
### 6. [Summary](#summary)

![image1](./images/movie_covers.jpg)

<a id='overview'></a>

# Overview

Using the __["small" dataset](https://grouplens.org/datasets/movielens/latest/)__ from __[MovieLens](https://movielens.org/)__, which contains explicit user ratings, movie titles, genres, etc., we were able to produce a model-based collaborative filtering recommendation system that allows for user input and will return the top 5 recommendations of movies from the dataset that the use has not yet rated.  Our process involved using the Surprise Python scikit library to process data and iterate through multiple recommender algorithms (including SVD and SVD++), using GridSearch, cross-validation and RMSE to decide on our best-performing model.  Our final model used a tuned SVD algorithm with an RMSE of 0.8464.  We also create a content-based filtering model, using TF-IDF Vectorizer and cosine similarity, to address the "cold start" problem inherent in collaborative filtering models.  With this model, a user who is not already in the dataset can input a known movie from the dataset and be returned 5 movie recommendations to choose from.

<a id='bidness'></a>

# Business and Data Understanding

The MovieLens small dataset contains 100,836 user ratings from 610 different users, each of whom contributed at least 20 ratings.  A total of 9,742 movie titles are included in this dataset.  There are two additional .csv files contained within the package download that we did not end up using.  One file contained 3,683 tags ("a single word or short phrase") that users applied with their numerical rating, which represented less than 4% of the total ratings in the dataset.  The other file contained links of each movie in the dataset to its listing on __[The Movie Database](https://www.themoviedb.org/)__ or on the __[Internet Movie Database](https://www.imdb.com/)__

The MovieLens dataset was specifically developed with recommendation system building in mind.  The data contains explicit user ratings, movie titles, and genres with consistent user ID and movie ID indices across files.  The business problem we were tasked with was to "build a model that provides top 5 movie recommendations to a user, based on their ratings of other movies".  Though movie recommendation systems are now common-place in the streaming apps we have available, understanding the architecture of these everyday models may allow us to expand their use into other realms, or at least refine what a model can currently provide, with the goal of delivering the most refined experience to an individual user.  

Citation included in the dataset's README.txt:  
F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4: 19:1–19:19. <https://doi.org/10.1145/2827872>

Additional citations included in our notebook.

<a id='dataprep'></a>

# Data Preparation:



<a id='modeling'></a>

# Modeling




<a id='final'></a>

# Final Model Evaluation


![Comparison of RMSEs from all algorithms tested](./images/suprise_models_bar.png)

<a id='summary'></a>

# Summary



For More Information
Please review the full analysis in our __[Jupyter Notebook](https://github.com/mccafj/MovieLens-Recommendation-System/blob/main/Final%20Notebook%20MovieLens%20Recommendation%20System.ipynb)__ or the __[PDF of our slide presentation.]()__

For any additional questions, please contact Samuel Robins sammyrobins305@gmail.com or Jon McCaffrey jonmccaffrey524@gmail.com

Repository Structure

###### ├── __[README.md](https://github.com/mccafj/MovieLens-Recommendation-System#readme)__
###### ├── __[Final Notebook MovieLens Recommendation System.ipynb](https://github.com/mccafj/MovieLens-Recommendation-System/blob/main/Final%20Notebook%20MovieLens%20Recommendation%20System.ipynb)__  <- Main notebook for project code
###### ├── __[slides.pdf]()__      <- PDF of slides for our presentation
###### ├── __[Data](https://github.com/mccafj/MovieLens-Recommendation-System/tree/main/data)__			                          <- Location of raw dataset
###### └── __[Images](https://github.com/mccafj/MovieLens-Recommendation-System/tree/main/images)__                              <- images used and generated in the project
