## Case-Study-CE880

## STEPS TAKE IN THE PROJECT



1. First, several libraries are imported, including pandas, sklearn, matplotlib, and seaborn. These libraries will be used throughout the code for tasks such as data manipulation, model fitting, and visualization.

2. The file data_banknote_authentication.txt is read into a Pandas dataframe, and the column names are changed to "variance", "skewness", "kurtosis", "entropy", and "class". The data is then saved to the file again with the updated column names.

3. Some basic information about the data is displayed, including the first few rows, the data types of the columns, and some summary statistics.

4. The data is visualized using histograms and density plots.

5. The data is checked for null values, and a boxplot is generated to identify any outliers.

6. The Pearson correlation coefficient between the different features is calculated and visualized using a heatmap.

7. The data is normalized using RobustScaler and PowerTransformer.

8. The data is split into training and testing sets using train_test_split.

9. A dictionary of different machine learning models is created, including LogisticRegression, KNeighborsClassifier, SVC, RandomForestClassifier, GradientBoostingClassifier, and XGBClassifier.

10. A function called model is defined, which fits each of the models to the training data, makes predictions on the test data, and prints out various evaluation metrics such as accuracy, AUC, and a classification report. The function also generates a confusion matrix to visualize the model's performance.

11. A function called estimator is defined, which loops through the models in the estimators dictionary and calls the model function on each one, passing in the training and testing data as arguments.

12. The estimator function is called, which fits and evaluates each of the models on the banknote authentication data.

## HOW TO RUN CODE

Data is already provided and import in the correct directory path.
clone repo and run notebook in jupyter notebook.
install any missing package with pip install. e.g pip install xgboost

13. The performance of the models is compared using a variety of evaluation metrics, including accuracy, auc, precision, recall, and f1-score.

## IN SUMMARY


The code in this notebook does the analysis of a dataset of banknote authentication data. It begins by generating histograms and a boxplot of the data using seaborn and matplotlib, respectively. It also computes the pairwise correlations between the features using the corr function from pandas and visualizes the correlations using a heatmap generated with seaborn.

The code is trying to get the data ready for analysis. It starts by changing the scale of two features called 'variance' and 'skewness' so that they are not affected by any unusual or extreme values that might be present. Then, it changes the shape of the distribution of two other features called 'kurtosis' and 'entropy' so that they are more evenly spread out and easier for the computer to understand. All of these changes are being made to help predict the data more accurately.

After preprocessing the data, the code splits it into training and test sets using the train_test_split function from scikit-learn. It then defines a dictionary of scikit-learn classifiers to be evaluated and a function that fits each classifier to the training data, makes predictions on the test data, and displays the resulting accuracy, AUC, classification report, and confusion matrix. Finally, it calls the function to evaluate each classifier on the test data. The results of the evaluation are printed to the console.
