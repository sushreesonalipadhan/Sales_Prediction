# Sales_Prediction
This project is to predict sales based on advertising expenditures across different platforms using a provided dataset. The dataset contains information on advertising spending for TV, Radio, and Newspaper, along with the corresponding sales figures.

1. Data Preprocessing :
The dataset was inspected for any missing values, outliers, and inconsistencies. Standard data cleaning techniques were applied where necessary.
Features were selected based on their relevance to the target variable (sales).
The data was split into training and testing sets using train_test_split from sklearn.model_selection to ensure an unbiased evaluation of the model.

2. Model Training :
A Linear Regression model was chosen due to its interpretability and simplicity for this task.
The model was trained on the training data using sklearn.linear_model.LinearRegression, with the aim of capturing the relationship between advertising expenditures and sales.
Feature scaling was considered, but given the nature of the data, it was determined unnecessary for this model.

3. Model Evaluation :
The model's performance was evaluated using the test set. Predictions were made based on advertising expenditure on TV using model.predict(X_test).
The accuracy of the model was assessed using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²).
Cross-validation was performed to ensure the model's robustness and generalizability.

4. Results Interpretation:
The model coefficients and intercept were obtained using model.coef_ and model.intercept_ to understand the contribution of each advertising platform to sales.
The predictions and actual sales values were visualized using matplotlib.pyplot.plot and matplotlib.pyplot.scatter to provide a clear comparison.
Residual plots were generated to analyze the distribution of errors and to check for any patterns that might suggest model inadequacies.
