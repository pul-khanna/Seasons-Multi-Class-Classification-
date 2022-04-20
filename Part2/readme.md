This part is divided into 2 files - 'Predict_Season_Wrangle_(Multi_Label).ipynb' and 'Predict_Season_Modelling_(Multi_Label).ipynb'.

Here the data wrangling operations are performed specifically for tree based models such as XGBoost, CatBoost etc

In the modelling file, we will demonstrate how to train a baseline XGBoost model and then fine tune the hyperparamters. 

We will also compare it to a baseline (default parameters) CatBoost Model and observe that the latter performs slightly better than tuned XGBoost model. The reason for this might be that most of our explanatory variables are categorical

Note: The wrangled data files are saved as 'season_train.csv' and 'season_test.csv' within the same folder (Part2)
