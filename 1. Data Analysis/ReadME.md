Before implementing any kind of data science project, you need to understand the data and the domain you are working in, which will influence the solution that you will create. In a real-world scenario, this is also a step where you should consider if you actually have all the data you need.

The goal of this milestone is to give you time to think about and understand the material you will be working with. Normally, recommender system algorithms come with a description of how well they performed on a specific dataset. It is great to know if they work, but unfortunately, this performance does not always transfer. A recommender algorithm can be excellent on one dataset and mediocre on another. Therefore, a first step to implementing a recommender system is to understand your data. This will also be key to understanding whether your algorithm is working or, if not, why.

# Objective

If you are working with a large dataset, you can’t study each data point and consider how exactly each rating influences a specific user. Instead, you have to attempt to get an overview of all the data and understand how the data is distributed. Your objective in this milestone is to get a feel for the dataset and understand the users and ratings.

Popularity is often mentioned in regard to movies and books. But what is popularity? Is a movie popular because it has been rated more times than any other movie five years ago? Your secondary objective in this milestone is to understand what popularity is.

# Importance to project

When you create a recommender system, you need to know the data, since the recommender will only ever be as good as the data used. If you don’t understand the data, you won’t be able to explain why the trained recommender system behaves as it does. And I can assure you, your boss will expect you to be able to explain why her eight-year-old daughter gets recommended horror movies or why your boss keeps getting sci-fi movies recommended.

In any data science project, if you don’t take the time to understand the data, you will often face much larger problems later.

# Workflow

1. Create a Jupyter notebook (take a look at the resources if you are new to this).
2. Load the data to be used from "MovieTweetings / latest."
    a. We will only use one of the three files, ratings.dat.
3. Answer the following questions:
    a. How many users and movies are mentioned in the dataset?
    b. How old are the data points (number of data points per year)?
    c. How popular are popular movies (based on the data, when would you say a movie is popular)?
    d. How many long-tail movies are there?
    e. How many movies has each user rated?
    f. If you had a recommender system that only recommended the most popular movies, how good would it be?
4. Write a report that answers the questions above and include charts to illustrate your answers.

# Deliverable

The deliverable for this milestone is a Jupyter notebook containing answers to the following questions:
a. How many users and movies are mentioned in the dataset?
b. How old are the data points (number of data points per year)? Create a bar chart that shows the age of the data points. Think about how old some of the data is and if it still makes sense to use it to understand taste.
c. How popular are popular movies (based on the data, when would you say a movie is popular)? Create a histogram showing how many movies are only rated once, two times, etc. This is to understand how many movies are rated many times.
d. How many long-tail movies are there? Think about the Pareto principle, and add a line in the histogram above that shows the longtail in this histogram.
e. How many movies has each user rated? Create a histogram that shows how many users have rated one more, two movies, etc.
f. How good would it be if you had a recommender system that only recommended the most popular movies?

Upload a link to your deliverable in the Submit Your Work section and click submit. After submitting, the Author’s solution and peer solutions will appear on the page for you to examine.