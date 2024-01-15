# About this project
The aim is to build a recommender system for the MovieGeek website.

The MovieGeek website was born in a DVD rental shop in England that was trying to survive a drop in customers in the brick and mortar shop. The owner of the shop always gave personalized recommendations to returning customers and hopes that you can replicate that on the website.

To be sure you can identify the customers’ preferences, you should start by doing a bit of data analysis on the available data. Using the data, you can then create charts that will help new customers see what movies are currently popular.

Returning customers should have recommendations based on their previous ratings of movies. You should use a collaborative filtering algorithm, non-negative matrix factorization, to implement the recommender. Finally, you will run the evaluation metric on the recommender and attempt to optimize it accordingly.

# Techniques employed
Listed under the bullets are the Python libraries for each technique.
- Investigating and analyzing the data we use
    - pandas: data manipulation and analysis
- Collaborative filtering with negative matrix factorization
    - scikit-learn: machine learning
- Visualizing the data in the reports
    - Matplotlib and seaborn: general visualization

# Project outline

In this liveProject, you will take on the task of adding a recommender system to a movie website.

The project is divided into four milestones.

1. Data Analysis
First, you will investigate the user movie rating data to gain an understanding of what to expect from your recommender system. Then you will produce a Jupyter notebook with your findings.

2. Non-Personalized Recommendations
With an understanding of the data, you will now implement charts to be used in different parts of the movie website. You will produce charts for each genre.

3. Personalized Recommendations
It is now time to implement personal recommendations based on the rating data. You will implement collaborative filtering using non-negative matrix factorization, produce personalized recommendations using latent vectors created by the factorization, and see them work on the running website.

4. Evaluation
Finally, you will evaluate the implemented recommendations algorithm and see if you can optimize a few of the hyperparameters. You will implement the evaluation and discuss it in a Jupyter notebook.

# Dataset
The dataset used in this liveProject is called MovieTweetings, and it consists of movie ratings found in well-structured tweets on Twitter. Since the dataset is updated continuously, you will be able to add your ratings to the dataset.

For more information, please refer to the ["MovieTweetings"](https://github.com/sidooms/MovieTweetings) repository.

# Technology versions

|Technology  |Minimum Version Required|Max Supported (Current) Version|
|------------|------------------------|-------------------------------|
|Python      |3.8                     |3.8                            |
|Django      |4.0                     |4.0                            |
|scikit-learn|1.0.1                   |1.0.1                          |

