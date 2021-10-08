# Recommender-System
![Python](https://img.shields.io/badge/Python-blue)
![Framework](https://img.shields.io/badge/Framework-Flask-yellow)
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-red)
![API](https://img.shields.io/badge/API-TMDB-fcba03)

demo: https://movieslr.herokuapp.com/

## Data Source

The datasets used:
1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)
6. [List of movies in 2021](https://en.wikipedia.org/wiki/List_of_American_films_of_2021)

I also use the api of https://www.themoviedb.org/ to get the details of each movie (title, genre, duration, rating, poster, etc) and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user on the IMDB site using "beautifulsoup" and performed sentiment analysis on those reviews.

## Recommender System

This is a content-based recommendation system that recommends movies similar to the ones the user likes. But how do you decide which item is most similar to the one the user likes?

## Similarity Score 

 It`s a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
 
 ## Cosine Similarity
 
 Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
 
 ![Cosine Similarity](https://user-images.githubusercontent.com/58336896/136577722-bb8fb099-56e4-47e8-93e9-6aed3df7e4bf.png)
