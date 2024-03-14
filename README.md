# classification-challenge
# Dylan Ross
1. Reads the data from the provided URL into a DataFrame.

2. Creates the labels set (y) from the “spam” column, and creates the features (X) DataFrame from the remaining columns.

3. Checks the balance of the labels variable (y) using value_counts.

4. Splits the data into training and testing datasets using train_test_split.

5. Creates an instance of StandardScaler; fits with the training and testing data.

6. Scales the training and testing features DataFrames using the transform function.

7. Creates a logistic regression model:

    A logistic regression model instance is created with a maximum number of iterations set to 10,000.
    The model is fitted to the scaled training data (`X_train_scaled` and `y_train`).
    The model's performance is evaluated using the `score` method, which computes the score for the training and testing datasets separately.

8. Creates a random forest model:

    A random forest model instance is created with 128 estimators and a random state set to 42.
    The model is fitted to the scaled training data (`X_train_scaled` and `y_train`).
    The score of the model is computed for both the training and testing datasets.

. Compare the performance of the logistic regression and random forest models:

    11.1. Determines which model performed better based on accuracy_score.
    11.2. Compares the actual performance with the predictions made earlier.
