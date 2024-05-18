# Recommender-System---Anime
Application of a basic RecSys to rate animes from MyAnimeList, based both on their description and genres, and using different types of RecSys.

## Content-Based RecSys
Content-Based RecSys makes use of features describing each anime, such as description and genres, in order to find the most similar animes to a given anime, here I provide two examples of content-based RecSys.

* In the Content-based file I make use of a fixed TF-IDF representation of each anime sypnopsis+genres in order to embed each anime, and then compute similarities score between every anime.
output: Given an anime j, this algorithm recommends the top k most similar animes to it. This algorithms DOES NOT MAKE USE of USER DATA.

* In the Matrix Factorization content-based algorithm I make use of a NN where I learn the embeddings for each item_ID and user_ID. In this case I'm making use of BOTH USER AND ITEM DATA.
output: Given a user j, this algorithms recommends the top k best items for that user.

## Knowledge-Based RecSys
Knowledge-Based RecSys are a conjunction of both RecSys and Information Retrieval.
Given a set of genres by the user as a string, the Knowledge-Based RecSys first eliminates animes which not contains those genres, and then computes the similarity between the encoded user input string 
and every item encoding, in order to pick the items that are most similar to the user specified parameters.


The original code was taken from Kevin Roitero's lectures on Recommender Systems, and adapted by me on different datasets

