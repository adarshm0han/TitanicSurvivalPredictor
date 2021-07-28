# Titanic Survival Predictor

##### This project was made for submission in Kaggle's "Titanic - Machine Learning from Disaster" competiotion.


## Objective

##### The goal of this model is to correctly predict if someone survived the Titanic shipwreak

## Dataset

##### The dataset was used for this model was obtained from Kaggle

## Solution
### Approach
##### Extensive data exploration was done to understand how numerical and categorical data was distributed and how different variables were related to each other.
##### Feature Engineering was done to see if a person's cabin, ticket, or their social status affected their rate of survival which was followed by data preprocessing. <br/>We wanted to drop null values, and include only relevent variables. We performed categorical transforms on all data so that the training and test data have the same columns. Calculated the mean for fare and age (could also use median). Normalised the fare and scaled the data in a 0-1 standard scaler.<br/>
##### The next step was to see how different models performed on our training set. The models used for our analysis were <br/>
Naive Bayes - 72.2%<br/>
Logistic Regression - 82.1%<br/>
Decision Tree - 77.6%<br/>
K Nearest Neighbor - 80.6%<br/>
Random Forest - 80.5%<br/>
Support Vector Classifier - 83.2% <br/>
Soft Voting Classifier - 81.5%<br/>

##### We implemented a soft voting classifier to calculate the average of the models, if a the average confidence was > 50% that it is a 1 it will be counted as such. <br/>

##### The model we finally used for prediction on our test set was the Soft Voting Classifier even though Support Vector Classifier had a better accuracy was because even though it perfoemed better on our training set, there is no guarantee that it will perform better on our test set.

## Result
##### As you can see, we were able to achieve an accuracy of 75.35% on the test set for the competition<br/>
![Capture](https://user-images.githubusercontent.com/84236742/127351906-daa45127-ecb9-47d6-b7ff-8309b3a4d039.PNG)
