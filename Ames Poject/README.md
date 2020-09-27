# Ames Housing Data

Ames Mini Project

I created a regression model based on the Ames Housing Dataset. This model predicts the price of a house at sale. The Ames Housing Dataset is an exceptionally detailed and robust dataset with over 70 columns of different features relating to houses. After cleaning and adding/removoing variables my final model had a total of 93 colunm


## Table of Contents
-[Problem Satatement](#problem-statement)

-[Set-up(Train)](#set-up-train)

-[The Modeling Process(Train)](#the-modeling-process-train)

-[Set-up(Test)](#set-up-test)

-[Testing the Model(Test)](#testing-the-moel-test)

-[Executive Summary](#executive-summary)

-[Slides](#slides)
 
 

## Problem Statement

We are hoping to build as accurate a model as possbile, based off the RMSE (Root Mean Squared Error) Score, given the housing data provided for Ames Iowa . 


## Set-up(Train)

1. Drop columns with excessive missing data that I do not fill comfortable with data.
2. Fill in missing values that I do fill confortable with fixing.
3. Create multiple dummy variables for my categorical variables that effectivly predict my model.
4. Create new polynomial varaibles that better predict my model such as Cond^2 and Cond multiplied by Gr Liv Area.

## The Modeling Process (Train)

1. Create X and y variables that best predict price.
2. split the data into a training set and testing set.
3. Create a pipeline to find what model best fits my data.
4. I used a Linear Regression model as it was better at prediciting then using Lasso
5. Review metrics on model to see the reliability of my new model.

## Set-up (Test)

Work with my Test data to make it the same shape as my train data so it fits my newly create model.
   
    1. Drop columns with excessive missing data that I do not fill comfortable with data.
    2. Fill in missing values that I do fill confortable with fixing.
    3. Create multiple dummy variables for my categorical variables that effectivly predict my model.
    4. Create new polynomial varaibles that better predict my model such as Cond^2 and Cond multiplied by Gr Liv Area.
    5. Create extra empty variables as there were two neighborhoods that did not exist in my test data
 
## Testing the model (Test) 
 
1. Create predictions off the model using test data.
2. Save and submit.
 
## Executive Summary

Given the model that we have created we can accuratle predict the price of a home given a multiple number of features roughly within $24,608 given the vast range and features of a home I am vary happy with this level of error. 

## Slides

See attathced slides for presentation on my model


