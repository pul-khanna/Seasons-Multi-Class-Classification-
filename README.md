# Seasons-Multi-Class-Classification-

This is a multi label classifictaion problem. The problem stated is a hypothetical one where an exoplanet with varying seasons has been discovered and a part of the data collected, of fruits growing in different weather conditions has got corrupted.

The dataset has been provided by Tredence. It has 42,748 rows and 14 columns.

The aim is to identify the type of climate the exoplanet has based on the properties of the fruit with the existing challenge of missing data.

The chosen metric for assessing/evaluating performance of the model is accuracy.

The modelling is divided into 2 parts:
*** (TO DO --- Add file from GoogleDrive)
Part 1:
We will start with a simple model of logistic regression as baseline and then compare with SVM and then Gradient Trees.
***

Part 2:
Here we will demonstrate how to train a baseline XGBoost model and then fine tune the hyperparamters. We will also compare it to a simple CatBoost Model.

Additional Info: 
We can try following methods which might further improve our scores:-
- Build model to handle missing values by predicting their values
- Feature Engineering (Create new features from given ones such as mean, deviations, interactions, etc) 
- Try using upsampling/downsampling techniques including SMOTE to handle unbalanced classes
- Build model within model (Notice season 'a' is 50% data, season 'u' is 38% and remaining other 2 seasons). e.g. We can build model 'a' vs rest and then   within that model 'u' vs rest and finally classify remaining 2 seasons
  and finally classify remaining 2 seasons. 
- Use Optuna library to tune the hyperparameters efficiently
- Use Permutation methods and/or SHAP values to determine most important features and use those

Note 1: The data wrangling and data modelling parts will be divided in 2 files for each each part. 

Note 2: Pay attentions to transformation and encoding methods as they will be different for models in Part 1 and Part 2 (Tree based models)

Note 3: The dataset is unbalanced and we will talk about different ways on how to build a model in such cases and demonstrate assigning weights to the classes method.
