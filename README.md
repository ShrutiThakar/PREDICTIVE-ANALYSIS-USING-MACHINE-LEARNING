# PREDICTIVE-ANALYSIS-USING-MACHINE-LEARNING

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: SHRUTI ASHOK THAKAR

*INTERN ID*: CT08DF1127

*DOMAIN*: DATA ANALYSIS

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*: This code, executed in a Jupyter Notebook or Google Colab environment, demonstrates a full end-to-end process for building and evaluating a linear regression model using synthetic data. It highlights key machine learning steps such as data generation, feature selection, model training, evaluation, and visualization, using libraries from Python’s data science ecosystem including scikit-learn, pandas, numpy, and matplotlib.

The code begins with the installation of essential packages using the command !pip install -q scikit-learn pandas matplotlib. This ensures that the machine learning library scikit-learn, the data manipulation library pandas, and the plotting library matplotlib are available in the runtime environment. These tools are crucial for handling data, creating models, evaluating performance, and generating visuals to interpret results.

The next step imports all necessary libraries. pandas and numpy are used for data manipulation, while matplotlib.pyplot is imported for data visualization. From scikit-learn, a variety of components are imported: make_regression for generating synthetic datasets; train_test_split for splitting data into training and testing sets; LinearRegression to create and train the model; SelectKBest and f_regression for feature selection; and multiple evaluation metrics including mean squared error (MSE), mean absolute error (MAE), and the R² score.

In Step 1, a synthetic regression dataset is created using make_regression(), which is useful for simulating real-world numerical data. The dataset contains 1,000 samples and 10 features, of which only 5 are informative — meaning they actually influence the target variable (y). A noise level of 15.0 is added to simulate data variability, which mirrors real-world conditions where data is not perfect. The features are labeled "feature_0" through "feature_9", and the target variable is named "target". This data is then assembled into a pandas DataFrame for easy inspection and manipulation.

In Step 2, feature selection is performed using SelectKBest along with the f_regression scoring function. This technique selects the top 5 features that are most strongly linearly correlated with the target variable. It evaluates each feature individually and selects those with the highest F-scores, which represent the ratio of variance explained by the feature to the variance not explained. The names of the selected features are printed, providing insights into which variables are most relevant for predicting the target.

Step 3 involves splitting the dataset into training and testing subsets using train_test_split. Here, 80% of the data is used for training, while the remaining 20% is set aside for testing. This separation ensures that the model is evaluated on data it hasn’t seen before, simulating how it might perform on real-world, unseen data.

In Step 4, a simple Linear Regression model is initialized and trained on the selected training data using the .fit() method. Linear regression attempts to find the best-fitting straight line through the data, minimizing the sum of squared errors between actual and predicted values.

Once trained, the model is used in Step 5 to make predictions on the test data. These predictions are stored in the y_pred variable. The performance of these predictions is evaluated in Step 6 using three standard metrics. The Mean Squared Error (MSE) measures the average squared difference between actual and predicted values; a lower MSE indicates better performance. The Mean Absolute Error (MAE) measures the average absolute difference between predicted and actual values, offering another perspective on error. The R² Score quantifies how well the model explains the variability in the target data — values closer to 1 imply a better fit.

Finally, Step 7 provides a visual analysis of the model’s performance. A scatter plot is generated comparing actual versus predicted values, with a red dashed line representing the ideal scenario where predictions perfectly match actual values. This visualization helps to intuitively understand the quality of the model — ideally, the scatter points should lie close to the red line.

In conclusion, this code effectively walks through a complete machine learning workflow using synthetic regression data. It introduces the concepts of feature relevance, model training, evaluation, and visualization in a simplified, reproducible environment. Such an approach is especially useful for beginners who want to understand core machine learning concepts before applying them to real-world datasets. Moreover, by using synthetic data and built-in tools from scikit-learn, the code maintains simplicity without sacrificing educational value, providing a clear understanding of regression modeling and performance assessment.


