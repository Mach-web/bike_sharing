# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### ANDERSON MACHARIA KINYUA

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The SampleSubmission needed to be converted to a DataFrame so as to add the predictions as a new column. Without doing so, the predictions would appear at the end of datetime column.

### What was the top ranked model that performed?
The last model with adjusted hyperparameters.

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
The train and test datasets were split according to days of the month and therefore days would not be a suitable predictor.

### How much better did your model preform after adding additional features and why do you think that is?
My public score improved from 1.79465 to 0.63665. The Year is highly correlated to the count. It is provides more predictive power.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The best tuned model had a score of 0.48056 which was the highest I could get.

### If you were given more time with this dataset, where do you think you would spend more time?
Feature engineering to get more predictive power from the features.

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
Feature engineering appears to be the most important part of model development. Adjusting the hyperparameters is an additional process that slightly improves the model.
