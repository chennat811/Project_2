# Project 2 - Prediciting the rating of documentaries using linear regression models


The goal of this project is to predict the Metacritic scores of documentaries to identify the documentaries that are worth watching. 


Data from IMDB and Box Office Mojo was used in the final model building and analysis. 


Initially, the Metacritic score was the main target, however the models created were not a great predictor of the Metacritic score. Therefore, a secondary target, User Rating - IMDB was used to build a model to see whether we could still identify the top documentaries with this metric. 

Features: From IMDB - Title, number of votes, release date, director, running time. From Box Office Mojo -  Max theaters, opening box, opening theaters, distributor, rank on box office mojo(by gross)

Target - Metacritic score, User Rating-IMDB

Tools Used - BeautifulSoup, Pandas, Matplotlib, Seaborn, Statsmodels, SKlearn


Results:
The best model for predicting the Metacritic score (range 0-100) was a linear regression model with log transformed features. The R2 on the training set was 0.323 and 0.226 for the test data. The MAE was 5.981 and RMSE was 7.355. The best model for predicting User rating-IMDB (range 0-10) was also a linear regression model with log transformed features. The R2 score for the training data was 0.344 and 0.166 for the test data. The MAE was 0.353 and RMSE was 0.469, therefore the model is generally 0.35 points away from the acutal rating, making it a decent predictor.

Possible impacts of your project - Be able to predict the Metacritic score or user rating.
