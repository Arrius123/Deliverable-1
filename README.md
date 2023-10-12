# Deliverable-1
code: https://colab.research.google.com/drive/1t42mA6PCgGTrcTndqMAWNO9GWZ2IKnif?usp=sharing



For this project, a Linear Regression model and a Decision Tree model will be used to analyze a movie dataset.

The first thing you want to do is import all of the necessary functions (numpy, pandas, matplotlib).

Then you want to import your google drive from colab.
Then you need to download the files below (they are too big to upload here) and put them in a colab folder:
https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset/data

When you have all 7 tables moved into your colab folder, you can set each of them equal to different varibles of your choosing.

You can then see each table by typing in the variables you choose for each table as inputs.
You can use the .decribe() function to find the statistical data on each table.
The functions .head(10) and .tail(10) can be used to see the first 10 entries and last 10 entries (respectively) of each table
You can use the .shape() function after each table you named to get the shape of the table.

.nunqique is a function used to find the the number of unique values in a table.
To see how many null values are in a table, use the isnull().sum().
You will then try to see which of the tables can be combined with one another. In order for this to happen, the tables have to have at least one column that they have in common.
If there no tables that can merge together, use the movie_metadata table (as it has the most information).

Drop any of the categorical data (columns with words instead of numbers) with the .drop() function.
Then clean the data by dropping any null values and duplicates (.dropna and .drop_duplicates respectively)

Choose the budget column for your X value and the revenue column for you y value.

Then import the right models for the assignment (LinearRegression, DecisionTreeClassifier and plot_tree, train_test_split, mean_squared_error)
use X_train, y_train, X_test and y_test for your train test split.
Then you want to define a learing model for your accuracy tests.
Then make sure all of the training and testing variables have the same number of samples so the model can be fitted into the training set.
Once that is fitted, you can use a variable to set a prediction on the X_test (predict_t = LG.predict(X_test), for example).

You can then find the mean squared error by using mean_squared_error(y_test, predict_t). This will teel you how much error the Linear Regression model has.

Then you can print out a graph using plt.scatter, plt.plot, plt.xlabel, plt.ylabel, plt.legend, and plt.show functions to get a linear regression graph.

For the decision tree model, find the testing accuracy by using the learning function with the training and testing variables (like for Linear Regression)

You can then plot the tree using plt.figure, plot_tree, and plt.show functions.

You should end up with something similar to the code linked above.
