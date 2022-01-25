# Capstone
Author: Deja Prade

# Overview

In this project, I build a toy recommendation system using the amazon e-commerce data. I develop a content-based recommendation model for recommendations to new customers and a collaborative filtering model for recommendations to existing customers. I provide the top five toy recommendations for new and existing customers.

# Business Understanding

Popcorn (our stakeholder) is a startup company that recently entered the movie streaming business. The video streaming market is rapidly growing worldwide. To compete with the market giants, such as Netflix, Hulu, or Amazon Prime, Popcorn tasked us to build for their platform a movie recommendation system. This recommendation engine is a powerful tool, especially for the video streaming business. For example, more than 80 percent of shows watched on Netflix came from Netflix recommendations. In this context, our project aims to develop a movie recommendation system for Popcorn that can effectively recommend movies and maximize customer satisfaction with Popcorn’s streaming service.

Data

We use the MovieLens data set. This data set (ml-latest-small) contains 102,377 ratings (5-star rating) and 3,476 tag applications created between March 29, 1996, and September 24, 2018. A total of 610 users and 9,742 movies are included.

The data set also includes movie genres (Action, Adventure, Animation, Children’s, Comedy, Crime, Documentary, Drama, Fantasy, Film-Noir, Horror, Musical, Mystery, Romance, Sci-Fi, Thriller, War, Western, and (no genres listed)).

All users had rated at least 20 movies. No demographic information is provided.

Model

We develop a content-based recommendation model based on movie genres and a collaborative filtering model based on user ratings. Content-based and collaborative filtering are two of the most common types of recommendation systems. Content-based recommendation systems focus on the items’ attributes, such as genres, and provide recommendations based on the similarity between them. In contrast, the collaborative filtering recommender is entirely based on a viewer’s history and not the context. It analyses how similar the taste of one user is to another and makes recommendations on that basis. Because collaborative filtering has a cold start problem, for the case of new users or new items, we build a content-based recommender. For the existing users, we build a collaborative filtering model.
