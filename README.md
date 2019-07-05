# Recommendations with IBM

In this project we anaylze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles you think they will like. The project is divided in five parts.

## System Requirements

You will need python 3.x and the following libraries:
- pandas
- numpy
matplotlib
- pickle
- seaborn
- collections


## I. Exploratory Data Analysis

Before making recommendations of any kind, we will need to explore the data you are working with for the project. 
For example the plot below show a right skewness for the articles read by users. 

![hist_of_interactions](https://github.com/NadimKawwa/ibm_recommendation/blob/master/plots/user_article_hist.png)

## II. Rank Based Recommendations

To get started in building recommendations, we will first find the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

## III. User-User Based Collaborative Filtering

In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users.

## IV. Content Based Recommendations (TBD)

Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. Using  NLP skills, we might come up with some extremely creative ways to develop a content based recommendation system. 
## V. Matrix Factorization

Finally, we will complete a machine learning approach to building recommendations. Using the user-item interactions, we will build out a matrix decomposition. Using our decomposition, we will get an idea of how well we can predict new articles an individual might interact with (spoiler alert - it isn't great). We will finally discuss which methods we might use moving forward, and how we might test how well your recommendations are working for engaging users.
