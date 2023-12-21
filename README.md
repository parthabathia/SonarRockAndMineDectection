# Sonar Rock and Mine Detection

This Python code is a machine learning script that uses logistic regression to classify data from a sonar dataset. Here's a breakdown of the code:

1. **Importing Dependencies:**
   - The code begins by importing necessary libraries such as pandas, numpy, scikit-learn's `train_test_split` for data splitting, `LogisticRegression` for creating a logistic regression model, and `accuracy_score` for evaluating the model's accuracy.

2. **Loading Dataset:**
   - The sonar dataset is loaded into a pandas DataFrame (`sonar_dataset`) from a CSV file named 'sonar_data.csv'. The dataset is assumed to have no header, as `header=None` is specified during the loading.

3. **Exploratory Data Analysis:**
   - The first five rows of the dataset are displayed using the `head()` method to give an overview of the data.
   - The code then prints the count of each unique value in the last column (column 60) of the dataset, assuming it contains the target labels.

4. **Data Preprocessing:**
   - The features (X) are created by dropping the last column (column 60), and the target variable (Y) is extracted.
   - The data is split into training and testing sets using the `train_test_split` function with a test size of 10%, stratification based on the target variable (Y), and a random seed for reproducibility.

5. **Model Training:**
   - A logistic regression model is instantiated (`model`) and trained on the training data using the `fit` method.

6. **Training Data Evaluation:**
   - The model's predictions are made on the training data, and the accuracy is calculated using the `accuracy_score` function.

7. **Testing Data Evaluation:**
   - Similarly, the model's predictions are made on the test data, and the accuracy on the test set is calculated.

8. **Prediction on Input Data:**
   - The code then takes the entire input data (`X`) and converts it to a NumPy array. The model is used to predict the labels for this input data.

9. **Post-prediction Analysis:**
   - The unique values predicted by the model and their respective counts are calculated using NumPy's `unique` function.

Overall, this script demonstrates a simple workflow for loading data, splitting it for training and testing, training a logistic regression model, and evaluating its performance on both training and testing datasets. Additionally, it provides predictions on a given input dataset and analyzes the distribution of predicted values.
