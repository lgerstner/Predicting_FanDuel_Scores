# Predicting FanDuel Scores

This project focuses on predicting whether or not a batter in baseball will score points as measured on FanDuel. The following outlines the steps of the project and the corresponding Jupyter Notebooks that are used for that step.

1. Scrape Batter Data - In this step a web scraper is created that gathers batter data from Baseball Reference. This source was chosen because it has many of the conventional baseball statistics as well as the batter's FanDuel score for a given game. (Scrape_Batter_Data.ipynb)

2. Feature Engineering - For the second step more features were created based on the data that was gathered from the web scraping. The goal of this notebook is to incorporate more features that can help predict a player's performance. (Feature_Engineering.ipynb)

3. Create Player Groups - The third step creates groups within the data. The purpose of this is to identify different types of batters, this is done because there are often very different types of batters, ones that hit many home runs, ones that hit for a high average, and everything in between. With this in mind it can be beneficial to split the data based on the batter type prior to creating a model. (Create_Player_Groups.ipynb)

4. Final Model Create & Analysis - The last step creates some basic models that can be used to predict whether or not a player will score any FanDuel points for a given game. The results of each model is compared to a baseline model. The baseline model is created by predicting that the batter will always score a positive amount of FanDuel points. (Final_Analysis.ipynb)

## Future Work

The next steps of this project would be to consider more features that could be used to do the modeling of the data. One set of features that could be used is a batter's career statistics, it could be useful to know a player's career batting average, or career OPS, in order to have a better prediction. Knowing these statistics would also be able to provide a way to understand whether or not a player is on a hot or cold streak. Since it is commonly thought that players are due if they have been cold or slumping for a bit it would be interesting to see if this is actually true. 

Other future work is to develop more in depth models. Currently the models that are being used are off the shelf models from the sklearn library. To develop these models further one step would be to do a train test split that has a better representation of the data's distribution. Another step to for model development is to do feature selection to find the most important features in the data. This would be extremely insightful as to what really drives a player's FanDuel score for a given game. 