# Predicting FanDuel Scores
***

This project focuses on predicting whether or not a batter in baseball will score points as measured on FanDuel. The following outlines the steps of the project and the corresponding Jupyter Notebooks that are used for that step.

1. Scrape Batter Data - In this step a web scraper is created that gathers batter data from Baseball Reference. This source was chosen because it has many of the conventional baseball statistics as well as the batter's FanDuel score for a given game. (Scrape_Batter_Data.ipynb)

2. Feature Engineering - For the second step more features were created based on the data that was gathered from the web scraping. The goal of this notebook is to incorporate more features that can help predict a player's performance. (Feature_Engineering.ipynb)

3. Create Player Groups - The third step creates groups within the data. The purpose of this is to identify different types of batters, this is done because there are often very different types of batters, ones that hit many home runs, ones that hit for a high average, and everything in between. With this in mind it can be beneficial to split the data based on the batter type prior to creating a model. (Create_Player_Groups.ipynb)

4. Final Model Create & Analysis - The last step creates some basic models that can be used to predict whether or not a player will score any FanDuel points for a given game. The results of each model is compared to a baseline model. The baseline model is created by predicting that the batter will always score a positive amount of FanDuel points. (Final_Analysis.ipynb)

## Future Work