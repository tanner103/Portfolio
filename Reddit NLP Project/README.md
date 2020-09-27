# Reddit NLP Project


## Table of Contents
-[Problem Satatement](#problem-statement)

-[Cleaning the Data](#pulling-and-cleaning-the-data)

-[Executive Summary](#executive-summary)

-[Conclusions and Recommendations](#user-content-conclusions-and-recommendations)

-[Slides](#slides)
 
 

## Problem Statement:

The goal of this project is to train a classifier using posts from two similar subreddits that will be able to classify correctly between the two subreddits. The data was pulled using Reddit's API and classified using both Naive Bayes and Random Forrest Classifier. The baseline for my model is 53% as that is that ratio of the largest category

My model is useful for anyone wanting to classify the subreddit of any post based on the text alone. The model is very flexible and subreddit someone might want.


## Pulling and Cleaning the Data:

1. Pulled 8,000 post from both the Movie & Books subreddit
2. Removed all removed post reducing my post to about 4,000 of each
3. Created a new column for text length
4. Combine data into a single dataset.
5. Remove all Null values
6. Remove outliers with over 6,000 word text
7. Final size of full DateFrame around  8,174 Saved in datasets as df
 
## Executive Summary:

For my two subreddits to build my model I have chosen r/movies and r/books. From a brief study of each subreddits I have found that they are quite similar in functionality and posts once key words are removed such as movie, film, book, page, etc. 

## Conclusions and Recommendations:

My first model included such words and the model preformed as follows:
   
   My Random Forest Classification was 96% accurate. This is a great score, but isn't very difficult given the number of key words helping the model. For example the word movie shows up of 6,000 times in this data set giving the model something very simple to make classifications on. I wanted to push my model further by removing these models and trying other classifiers.

To better compare these two subreddits and to increase the complexity of predicting I removed all of these key words in addition to all standard English stop words. The list of removed words are as followed: 'book' ,'books' ,'page' ,'chapter' ,'movie' ,'movies' ,'film' ,'films' ,'filmed', 'novel', 'Hollywood', 'camera', 'read', 'seen', 'saw', 'pages' ,'author' ,'authors' ,'watch', 'watched', 've', 'reading', 'https', 'com'. Removing these words makes all post between the two more difficult to distinguish so I put my model to the test. 

My final model preformed as follows:
      My Naive Bayes model had an accuracy score of 90% which I am super happy with given the likeness of the two separate data sets. The Naive Bayes became the better model for classification and I would highly recommend it's use for Natural Language Processing


## Slides:

See attached slides for presentation on my model


