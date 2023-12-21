#Sonar Rock and Mine Detection

This code analyzes a diabetes dataset to build a model for predicting whether a person has diabetes based on various medical features. Here's a breakdown of the steps:

    Data Import and Exploration:
        Libraries: Imports necessary libraries like Pandas, NumPy, Scikit-learn for data manipulation, scaling, and machine learning.
        Dataset Loading: Reads the diabetes dataset (diabetes.csv) using Pandas.
        Data Preview: Prints the first few rows of the dataset to get a glimpse of the data.

    Data Preprocessing:
        Feature Selection: Creates separate matrices for features (X) and target variable (Y - "Outcome").
        Data Scaling: Standardizes the features using StandardScaler for better model performance.
        Class Distribution: Prints the number of instances for each class ("Outcome") to understand the imbalance (if any).

    Model Training and Evaluation:
        Train-Test Split: Splits the data into training (80%) and testing (20%) sets to avoid overfitting the model.
        Model Training: Trains a Linear Support Vector Machine (SVM) classifier on the training data.
        Accuracy Evaluation: Calculates and prints the accuracy of the model on both training and testing data.

    Predictions on New Data:
        Input Data: Defines a list of new data points with medical features for six individuals.
        Prediction: Uses the trained model to predict the "Outcome" (diabetes) for each new data point.
        Results: Prints the predicted class and the count of each predicted class for the new data.

Overall, this code demonstrates the process of building and evaluating a machine learning model for diabetes prediction using a Support Vector Machine. By analyzing a diabetes dataset, the model can learn to identify patterns in medical features and predict the likelihood of diabetes for new patients.
Calculates the accuracy of the model on both training and testing data.
Shows that the model performs slightly better on the training data (83%) compared to the testing data (76%).

Predicts on new data: Allows prediction of the target variable for any new data point by providing its features as input.


Overall, this code demonstrates building and evaluating a Logistic Regression model for classifying sonar signals as mines ("M") or rocks ("R").
