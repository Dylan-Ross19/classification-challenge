# classification-challenge
# Dylan Ross
1. Reads the data from the provided URL into a DataFrame.

2. Makes a prediction as to which model you expect to do better (Logistic Regression or Random Forest).

3. Creates the labels set (y) from the “spam” column, and creates the features (X) DataFrame from the remaining columns.

4. Checks the balance of the labels variable (y) using value_counts.

5. Splits the data into training and testing datasets using train_test_split.

6. Creates an instance of StandardScaler.

7. Fits the Standard Scaler with the training data.

8. Scales the training and testing features DataFrames using the transform function.

9. Creates a logistic regression model:

    9.1. Creates a logistic regression model instance.
    9.2. Fits the logistic regression model to the scaled training data.
    9.3. Predicts labels for the testing data using the fitted model.
    9.4. Evaluates the model's performance using accuracy_score.

10. Creates a random forest model:

    10.1. Creates a random forest model instance.
    10.2. Fits the random forest model to the scaled training data.
    10.3. Predicts labels for the testing data using the fitted model.
    10.4. Evaluates the model's performance using accuracy_score.

11. Compare the performance of the logistic regression and random forest models:

    11.1. Determines which model performed better based on accuracy_score.
    11.2. Compares the actual performance with the prediction made earlier.
