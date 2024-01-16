# Non-Personalized Recommendations

We cannot personalize recommendations on our website for a user whom we know nothing about. No data means no personalization.

However, even if we don’t know anything about a particular user, we still have data about users in general. We can use that data to show the movies that are the most popular in hopes that the user is like everybody else and will enjoy those.

In this milestone, you will create a chart that shows the most popular items. But what is a popular item? That is the first question you should ask. Is it the item with the most ratings or the highest ratings?

You could also consider whether the most popular items are more controversial and determine which items have the highest variance in ratings.

There are many options, so the first thing you should do is settle on one and then implement it and see how it looks. Then, if time permits, try something else and compare.

When a user looks at a specific genre of movies, a chart should only show movies in that category (or perhaps similar categories). Implement a filter that will only show relevant movies for the category. Consider using rules like the following:

For animated movies, show a chart of movies from the animated genre, as well as family movies.

## Objective

It’s important to use the knowledge you have. The best thing we can do when we know nothing about a user is to use the data to create non-personalized charts.

## Importance to project

You will often need to create recommendations even when you don’t know much about the users. This is called a cold start problem. No user data means no personalized recommendations, but, with charts, you should be able to provide recommendations that will satisfy the majority of users.

## Workflow

1. As discussed above, the first thing we need to do is decide how to define what popular content is.
2. Create a Jupyter notebook.
3. Import the data. For this milestone, we will use two of the files from MovieTweetings:
    a. ratings.dat
    b. movies.dat
4. Do any data cleaning necessary based on the approach you have decided on.
5. It is not always the fastest or best to calculate which content to show when requested. Rather, it is a good idea to pre-calculate it. In the Jupyter notebook, implement the calculation of the charts:
    a. Global chart (for the landing page)
    b. One for each sub-genre
6. Create a Python dictionary, which is a list of key/value pairs. Each pair should contain the name of a genre and the corresponding top 10. Keys should be strings, and values should be DataFrames with the following schema: index::movie_id::movie_title::number_ratings
7. Save each of the charts in a folder called “charts” in the root of the liveProject (you need to create the folder).
8. Check that your saved charts will be loaded in the method to read the calculated results and respond in the rec API found [here](https://liveproject.manning.com/liveproject/git/live-project/recs/live_project_popularity_recommender.py).
9. Install the MovieGeek website:
    a. Clone the GitHub "live-project" repo.
    b. Create an ID for themoviedb.org (you have to create an ID with themoviedb.org to use its pictures).
        - Go to www.themoviedb.org.
        - Sign up.
        - Log in, go to your account settings, and create an API. You can access the settings by clicking the avatar in the upper right-hand corner (the default is a blue circle with a white logo in it). Then you’ll see the settings on the left.
        - Create a file in the MovieGeek directory called ".prs".
        - Open .prs and add the following:
            `{ "themoviedb_apikey": }`
        - Remember to remove the “<” and ">". When you are finished, the file contents should look something like this:
            `{"themoviedb_apikey": "6d88c9a24b1bc9a60b374d3fe2cd92ac"}`
10. Run the MovieGeek website:
    a. If you don’t have Docker installed, install it by following the instructions found in "Get Started with Docker."
    b. Open a terminal and go to the “live-project” folder (the folder that contains the docker-compose.yml file).
    c. Execute docker-compose build web.
    d. Then, execute docker-compose up web.
    e. It should output a link to the website. Copy-paste the URL (in my case, it’s http://0.0.0.0:8010) into a browser. On the website, you should see the MovieGeeks landing page with a chart to the right of the page.
11. Write a short report describing the following:
    a. The non-personalized feature you have implemented
    b. Your chart calculation method
    c. Your implementation
    d. How the genre charts look
    e. What you would improve given more time

## Deliverable

In this milestone you implemented a non-personalized recommender. The code and the implementation are, of course, the most important part and should already be in a Jupyter notebook. But to understand if it works well, it’s also important to evaluate how the calculated recommendations look. The deliverable is, therefore, both the notebook with the code, but the notebook should also include a description of what you have done, containing, at a minimum, a description of the following:
- The non-personalized feature you have implemented
    - What data did you use?
    - How often should it be recalculated?
- Your chart calculation method:
    - Consider how it would look if you only used last year’s data compared to all the data?
- How the genre charts look
    - Show examples of how it looks for one or two genres.
- What you would improve given more time

A report is an excellent way to show off your work—why not write a blog post about it?

Upload a link to your deliverable in the Submit Your Work section and click submit. After submitting, the Author’s solution and peer solutions will appear on the page for you to examine.