#Sonar Rock and Mine Detection

This code performs binary classification on sonar data to distinguish between mines and rocks. It uses a Logistic Regression model and evaluates its performance on both training and test data.

Here's a breakdown of the steps:

Import libraries: Essential libraries like pandas, numpy, sklearn for model selection, train-test split, and accuracy metrics are imported.
Load data: The sonar data is loaded from a CSV file into a pandas DataFrame.
Data exploration: The first 5 rows and class distribution (M for mines, R for rocks) are explored.
Feature engineering: The last column containing the class labels is separated into the target variable Y. The remaining columns become the features in X.
Train-test split: The data is split into training and testing sets for model training and evaluation. Stratified sampling ensures balanced class distribution in both sets.
Model training: A Logistic Regression model is trained on the training data.
Evaluation:
Training data accuracy: The model's performance on the training data is evaluated using accuracy score.
Testing data accuracy: The model's performance on unseen data is evaluated on the test set.
Prediction: The code allows predicting the class of new sonar data by:
Reshaping the input data to a NumPy array.
Using the trained model to predict the class ("M" or "R").
Overall, this code demonstrates the use of Logistic Regression for classifying sonar data and evaluating its effectiveness on both training and testing data.
