## Problem Statement

My goal is to use natural language processing to improve DrafKings targeted marketing strategy. I am attempting to make a model that can differentiate between football enthusiasts and fantasy football enthusiasts. This will allow the company to spend less money on advertising and reach the audience they are looking for. To do this I will take comments from the nfl subreddit and fantasy football subreddit, and create models to predict the subreddit based on the words used in the comments.


## Data Dictionary

|Feature|Type|Description|
|---|---|---|
|subreddit|string|The subreddit that the comment was posted in. This was the variable I was trying to predict|
|day_posted|int|The day that the comment was posted 0 is Monday, 6 is Sunday|
|body|string|The text of the comment|

---

## Summary

I first created a scraper to scrape the top 100 comments from both subreddits every day for the months of October and November of 2020. I chose October and November because those months are the peaks of the nfl and fantasy football seasons. I did some data analysis on the top words per subreddit and the days with the most activity. I then vectorized the comments. I made some models using stemmers but they performed worse than those without. I made three types of models, KNN, Random Forest, and Logistic Regression. The Logistic Regression model performed the best of these so I did further interpretation of this model.

---

## Conclusions

People are more likely to talk about football on days that games are not being played if they are interested in fantasy football. Fantasy football players are also more likely to talk about individual players who perform well statisically. There are also terms that fantasy football players will use when evaluating players and those could be used to target fantasy football enthusiasts. NFL fans are more likely to be talking about special teams players and college prospects. I would reccomend using my Logistic regression for targeted advertising as it has a 70% accuracy and could save the company a lot of money while reaching most fantasy football fans.