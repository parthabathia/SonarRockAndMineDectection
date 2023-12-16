#Sonar Rock and Mine Detection

This code is written in Python and performs the following tasks:

Imports necessary libraries: Including pandas, numpy, scikit-learn libraries for data manipulation, model training, and evaluation.

Loads data: 

Reads sonar data from a CSV file into a pandas dataframe.

Prepares data:

Checks the distribution of the target variable ("60th column"). It shows two categories: "M" and "R".

Separates features (all columns except the last) and the target variable.
Splits the data into training and testing sets, ensuring the target variable distribution is preserved (stratified sampling).

Trains a Logistic Regression model: Uses the training data to train a Logistic Regression model to predict the target variable ("M" or "R").

Evaluates model performance:

Calculates the accuracy of the model on both training and testing data.
Shows that the model performs slightly better on the training data (83%) compared to the testing data (76%).

Predicts on new data: Allows prediction of the target variable for any new data point by providing its features as input.


Overall, this code demonstrates building and evaluating a Logistic Regression model for classifying sonar signals as mines ("M") or rocks ("R").
