# Recommender-System---Anime
Application of a basic RecSys to rate animes from MyAnimeList, based both on their description and genres, and using different types of RecSys.

## Content-Based RecSys
Content-Based RecSys makes use of features describing each anime, such as description and genres, in order to find the most similar animes to a given anime

## Knowledge-Based RecSys
Knowledge-Based RecSys are a conjunction of both RecSys and Information Retrieval.
Given a set of genres by the user as a string, the Knowledge-Based RecSys first eliminates animes which not contains those genres, and then computes the similarity between the encoded user input string 
and every item encoding, in order to pick the items that are most similar to the user specified parameters.


The original code was taken from Kevin Roitero's lectures on Recommender Systems, and adapted by me on different datasets

