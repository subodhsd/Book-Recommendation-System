# Book-Recommendation-System

### In this project we have used three different datasets to come up with a book recommendation system for different users based on how they and others have rated previously purchased books.

Tags: Recommendation Systems, Data Science, Machine Learning, Collaborative Filtering

Co-created by - @kasmin

## Project Files
This Project includes 1 Colab notebook, 1 Technical Document as well as 1 Presentation PDF

### Executable Files:
   Book_recomndation_system_final.ipynb - Includes all functions required for clustering operations.
   


## Abstract
During a last couple of decades, with the upward push of Youtube, Amazon, Netflix, and many different internet services, recommender systems have taken a very important place in our lives. 

   In a totally trendy way, recommender systems are algorithms aimed toward suggesting applicable objects to users (items being films to watch, textual content to read, merchandise to buy, or whatever else relying on industries
   
## Problem Statement
Recommender systems are really critical in some industries as they can generate a  huge amount of income when they are efficient or also be a way to stand out  significantly from competitors. 

The main objective is to create a machine learning model to recommend relevant books to users based on popularity and user interests. 

## Introduction
Recommender systems are truly important in a few industries as they could generate a massive quantity of profits whilst they may be efficient or additionally be a way to stand out notably from competitors.

From e-commerce (propose to consumers articles that might hobby them) to online advertisement (propose to customers the proper contents, matching their preferences), recommender systems are these days unavoidable in our everyday online journey.

## Exploratory Data Analysis
The number one purpose of EDA is to guide the analysis of facts previous to making any conclusions. It may also useful resource withinside the detection of obvious errors, in addition to a deeper knowledge of facts patterns, the detection of outliers or anomalous events, and the discovery. Followings are the observations from EDA.
1) Agatha Christie is the Top authors with highest numbers of book
2) Harlequin is the Top Publisher with highest numbers of book
3) USA is the Top Country with highest numbers of users
4) There are some outlier in the age column. majority of the users are of age 20-35 
5) Maximum of book have good rating.8 is the most common rating for most number of book

## Feature Engineering
1) From the analysis part we get that the Year-Of-Publication was wrongly  mentioned for some of the rows. 
2) Diving deep into the Books dataframe we got to know that for these rows  there was actually a column mismatch. 

## Algorithms Used
### Popularity Based Recommendation
It is a sort of recommendation system which fits at the precept of popularity and or something that's in fashion. These structures test approximately the books that are in trend or are maximum famous many of the customers and without delay recommend them. For example, if a product is regularly bought with the aid of using maximum people then the system gets to recognizes that that product is maximum famous so for each new consumer who simply signed it, the system will recommend that product to that consumer additionally and probabilities become excessive that the brand new consumer will even buy that. Using this recognition metric we are able to calculate the top books that might be recommended to a consumer. 

Our Popularity score formula-
popularity_score=0.7*Avg_rating+0.3*Rating_count 

Avg_rating=Average rating of the book

Rating_count=Number of rating of the book

### Collaborative Based Filtering
In Collaborative Filtering, we generally tend to discover comparable customers and advise what similar customers like. In this sort of recommendation system, we don’t use the features of the item to advise it, as an alternative we classify the customers into clusters of comparable types and recommend every person consistent with the choice of its cluster.

1) Cosine similarity:  Similarity degree refers to distance with dimensions representing features of the data object, in a dataset. If this distance is less, there might be an excessive degree of similarity, however whilst the space is large, there might be a low degree of similarity. In this assignment, I actually have used ‘Cosine Similarity’ that is a famous similarity degree. Cosine similarity is a metric, beneficial in determining, how comparable the information items are regardless of their size. In cosine similarity, information items in a dataset are dealt with as a vector.

2) Singular value decomposition: The Singular Value Decomposition (SVD) of a matrix is a factorization of that matrix into 3 matrices. It has a few interesting algebraic properties and conveys vital geometrical and theoretical insights approximately linear transformations. It additionally has a few vital packages in data science. 

## Evaluation of SVD model using Recall @k 
T MAP@K offers perception into how relevant the listing of recommended items are, while MAR@K offers perception into how nicely the recommender is capable of recoll all of the items the person has rated definitely withinside the test set.

## Conclusion

1) Majority of the readers were of the age bracket 20–35 and most of them came from North  American and European countries namely USA, Canada, UK, Germany and Spain. 

2) Author of most of the books was Agatha Christie, William Shakespeare, Stephen King

3) 8 is the most common rating for most number of book. Rating below 5 are in very few in number. 

4) MAR@K gives  that our SVD recommender is able to recall much more then random Recommender. 

