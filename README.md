# PRODIGY_ML_01
House Price Prediction with Linear Regression This code implements a linear regression model to predict house prices based on their square footage (GrLivArea), number of bedrooms above ground (BedroomAbvGr), and number of full bathrooms (FullBath).

Dependencies:

NumPy
pandas
scikit-learn
Data Source:

Kaggle dataset: "House Prices: Advanced Regression Techniques" (https://www.kaggle.com/datasets/yasserh/housing-prices-dataset) (Note: You'll need to download the data and place it in the path specified in the code)
Process:

Load Data: Reads the CSV data from the specified path.
Data Cleaning: Removes rows containing missing values for the chosen features: square footage, bedrooms above ground, full bathrooms, and sale price.
Feature Selection: Isolates the chosen features (X) and the target variable (sale price, y) from the cleaned data.
Train-Test Split: Splits the data into training and testing sets using train_test_split from scikit-learn. The training set is used to fit the model, and the testing set is used to evaluate its performance.
Model Creation and Training: Initializes a linear regression model (LinearRegression) and trains it using the training data.
Prediction: Makes price predictions on the testing set using the trained model.
Evaluation: Computes the R-squared score and mean squared error (MSE) to assess model performance. R-squared indicates the proportion of variance in the target variable explained by the model, while MSE measures the average squared difference between predicted and actual values.
Display Predictions: Creates a DataFrame showing both actual and predicted house prices for the testing set.

Example Output:

R-squared score: 0.75  
Mean Squared Error: 123456.78 

           Actual      Predicted
0      1234567.0  1189034.21
1       876543.2   901234.56

Disclaimer:

This is a basic example using linear regression. House prices are influenced by various factors beyond the three considered here. More features and advanced machine-learning techniques may be needed for improved accuracy in real-world scenarios.
