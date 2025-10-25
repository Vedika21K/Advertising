Advertising Regularization with SciKit-Learn
This project explores the application of regularization techniques (Ridge, Lasso, and Elastic Net) using SciKit-Learn to improve a linear regression model on the Advertising dataset.

Data
The dataset used is the "Advertising.csv" file, which contains information about the money spent on TV, Radio, and Newspaper advertising and the corresponding sales.

Methodology
Polynomial Feature Conversion: The original features were converted into polynomial features of degree 3 to capture non-linear relationships.
Train | Test Split: The data was split into training and testing sets to evaluate the model's performance on unseen data.
Data Scaling: The features were scaled using StandardScaler to ensure that all features contribute equally to the model training.
Model Training and Evaluation:
Ridge Regression: A Ridge regression model with cross-validation (RidgeCV) was trained to find the optimal alpha value.
Lasso Regression: A Lasso regression model with cross-validation (LassoCV) was trained to find the optimal alpha value.
Elastic Net: An Elastic Net model with cross-validation (ElasticNetCV) was trained to find the optimal L1 ratio and alpha.
Performance Evaluation: The models were evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) on the test set.
Results
The performance of each model on the test set is summarized below:

Ridge Regression:
MAE: 0.4273774884328613
RMSE: 0.6180719926962934
Best Alpha:  0.1
Lasso Regression:
MAE: 0.6541723161252868
RMSE: 1.1308001022762548
Elastic Net:
MAE: 0.566326211756945
RMSE: 0.7485546215633726
Best L1 Ratio: 0.7485546215633726
Based on the MAE and RMSE values, the Ridge regression model performed the best on this dataset.