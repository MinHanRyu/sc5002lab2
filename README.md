# SC5002 Lab 2

This lab uses the automobile data set obtained [here](https://archive.ics.uci.edu/dataset/10/automobile).

## Steps
1.  Setting up virtual environment
A `requirements.txt` file was generated from the virtual environment.

2. Dataset loading
The dataset was loaded using `pd.read_csv` and using the link as a argument.

3. Imputation for missing data
Two approaches were used for dealing with missing data. For numerical data, the median was used to simply fill the missing data. For categorical data, the mode was used to fill the missing data. The variables/columns with data was found using dataframe indexing.

4. Encoding categorical data
To handle the nominal data (which has no order), one-hot encoding was used. To handle the ordinal data, label encoding was done to label a unique integer to each cataegory in specific columns.

5. Split into training/test
As per regular ML practice, the training and test set was split with a 20% test ratio.

6. Fit Linear Regression model and Ridge Regression model in same Training data. Alpha equal to 1 give a moderate level of regulaization.

7. Then, I used the trained model to predict y_test (Price) and compared the Predicted y_test and actual y_test using a scatterplot.

8. Import all libraries and set up K-fold cross validation. First, test and train using cross validation and calculate CV score and R^2. For Rige resgression, we create loop through using different alpha to train and test using cross-validation for each alpha and get CV score and mean score. Then plot graph to visualise ridge regresssion with different alpha with mean cross-validation score.

9. Calculating the Mean Squared Error (MSE) and R² score
We first train the 2 models, Linear Regression and Ridge Regression. After training the models, we then start to calculate the MSE and R² and print out the results for the test

10. Checking for Overfitting & Preventing it
We check the performance using the MSE and R² score for both models by calculating both test and train and comparing the values of coefficients. If there are large differences between training and test, it will indicate overfitting

11. Improving Model Performance
When the alpha value is small, the regularization effect is minimal, and the model behaves similarly to linear regression. When the alpha value is large, the regularization becomes stronger, shrinking the coefficients (β) toward zero. This prevents the model from fitting noise in the training data, improving generalization to unseen data, but also potentially underfitting the data if α is too large.

12. When to use Linear Regression: 
a. Small to moderate number of features
b. No Overfitting Issues
c. Simplicity & Interpretability

Practical Applications:
a. House Price Prediction
b. Sales Forecasting
c. Medical Cost Prediction

13. When to use Ridge Regression:
a. High number of features or when multicollinearity exists
b. Regularization Needed to prevent overfitting
c. Better Generalisation

### Practical Applications:
a. Predicting Stock Prices
b. Genomic Data
c. Customer Segmentation in Marketing
d. Financial Risk Modelling

