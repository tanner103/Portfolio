# THIS PROJECT IS UNDER CONSTRUCTION


# The All-Star Effect

<h1 align="center">
  <br>
  <img src="https://turbologo.com/articles/wp-content/uploads/2019/10/NBA-logo-illustration-678x381.jpg.webp" alt="NBA" width="360">
</h1>


## Table of Contents

-[Problem Statement](#problem-statement)

-[Cleaning the Data](#pulling)

-[Data Dictionary](#data-dictionary)

-[Executive Summary](#executive-summary)

-[Conclusions and Recommendations](#user-content-conclusions-and-recommendations)

-[Slides](#slides)
 
 

## Problem Statement:

The NBA's All-Star game has been around since 1951. This game is hosted every February by the National Basketball Association and showcases 24 of the league's star players. The starting lineup for each squad is selected by a combination of fan, player, and media voting, while head coaches choose the reserves, making in the end a 12-man roster for each team.

Since the All-Star game is considered to have no impact on the actual season it usually isn't a competitive game and is a more casual viewing experience for fans. 

The goal of this project is to prove that there is a lot more to be considered behind what it mean to be an All-Star and the potential effects it could have on the rest of the season. 


## Pulling:

1. All player data, outside of the All-Star status, was pulled from nba.com using Selenium and BeautifulSoup to scrape the data.
2. The All-Star status was built from information off of espn.com.
3. The final data set included all player stats from 00-01 season to the 18-19 season and consisted of just under 9,000 observations.


## Data Dictionary

| Abbreviation | Definition |
|---|---|
|GP |Games Played 
|W |Wins 
|L |Losses 
|MIN |Minutes Played 
|FGM |Field Goals Made 
|FGA |Field Goals Attempted 
|FG% |Field Goal Percentage 
|3PM |3 Point Field Goals Made 
|3PA |3 Point Field Goals Attempted 
|3P% |3 Point Field Goals Percentage 
|FTM |Free Throws Made 
|FTA |Free Throws Attempted 
|FT% |Free Throw Percentage 
|OREB |Offensive Rebounds 
|DREB |Defensive Rebounds 
|REB |Rebounds AST Assists 
|TOV |Turnovers 
|STL |Steals 
|BLK |Blocks 
|PF |Personal Fouls 
|FP |Fantasy Points 
|DD2 |Double doubles 
|TD3 |Triple doubles 
|PTS |Points 
|+/- |Plus Minus Ratio

 
## Executive Summary:

I will first attempt to properly classify if a player is an All-Star or not based solely on their stats for the season. 

Next I will look at what key factors go into this classification and use them to create a regression to see if I can properly predict these features and see the effect of being an All-Star highly influences these factors.

## Conclusions and Recommendations:

In my classification I attempt to use the following models with the following conclusion.

    Logistical Regression: 97.31 Accuracy

    Random Forest Classifier: 97.58 Accuracy

    Support Vector Classifier: 90.88 Accuracy

    Neural Network: 97.27 Accuracy

Due to the high accuracy of all my models I stuck with the logistical regression since it gives me interpretable coefficients. From our results we can see...

Based off of these results I wanted to see, holding all other variables constant, the effect of being an All-Star had on the number of free-throws taken. To do this I ran a Linear Model removing variables like PTS, FTM, FP, GP. My finl results were:

    Train Score: .87

    Test Score: .86
    
My Model returned All_Star with a coefficient of 76.87. That is to say that being an All-Star in the NBA inceases your Free Throw Attemps count by roughly 77 shots. 
 

## Slides:

See attached slides for presentation on my model


