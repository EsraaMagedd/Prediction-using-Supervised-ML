# Prediction-using-Supervised-ML
Predicting the percentage of a student based on the no. of study hours

This code performs a simple linear regression analysis to predict a student's percentage score based on the number of hours they studied. It uses the Python machine learning library scikit-learn to split data into training and testing sets, train the algorithm, and predict test set results.

To begin, the necessary libraries are imported, including pandas, numpy, and matplotlib.pyplot. The data is then imported from a remote CSV file using pandas, and a brief analysis of the data is conducted using data.head() and data.describe().

The data is then visualized using a scatter plot, with hours studied on the x-axis and percentage scored on the y-axis. The plot is given a title and axis labels before being shown using matplotlib.pyplot.show().

The data is split into training and testing sets using the train_test_split function from scikit-learn. The independent variable x consists of all the values in the first column (hours studied), and the dependent variable y consists of all the values in the second column (percentage scored). The test set size is set to 20%, and the random_state parameter is set to 0 for reproducibility.

The algorithm is then trained using the LinearRegression class from scikit-learn, and fit to the training set using the regressor.fit() method. The training set results are then visualized using a scatter plot of the training set data points in red, and a blue line representing the predicted scores.

The algorithm is then used to predict test set results using the regressor.predict() method, and the results are visualized using a scatter plot of the test set data points in red, and a blue line representing the predicted scores. The plot is given a title and axis labels before being shown using matplotlib.pyplot.show().

Finally, the algorithm is used to predict the percentage score for a student who studies for 9.25 hours, using the regressor.predict() method and passing in the single value as a two-dimensional array using double brackets. The result is then printed to the console in a formatted string.

Overall, this code provides a simple example of how to perform a linear regression analysis using scikit-learn in Python.
