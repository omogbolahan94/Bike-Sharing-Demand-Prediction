# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
I first ran the model, all of the predicted values were possitive so didn't need to change all negative values to zero.

### What was the top ranked model that performed?
WeightedEnsemble_L2

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I converted the `datetime` feature type from `object` to pandas `datetime` object and extracted the only the hour section from the feature and later droped the datetime feature itself. I also converted `weather` and `season`features from `object` type to `category` type.

### How much better did your model preform after adding additional features and why do you think that is?
Adding a new featured reduced the error by `1.29802`. A good linear regression model that is evaluated with Root Mean Squared Error (RMSE) metric will have a lower RMSE value. 

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: Add your explanation

### If you were given more time with this dataset, where do you think you would spend more time?
I would spend more time to understand the data and try different new engineered features. With more compute, I would try different hyper parameters and allocate more time limit for better performance.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|?|?|?|?|
|add_features|?|?|?|?|
|hpo|?|?|?|?|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
