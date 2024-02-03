# Code Documentation Machine Learning Final Exam
## Background
S&P 500 is a stock index consisting of 500 large companies from United States (US), which represents most of US stock market and represents company business performance in US.
Because of that, S&P 500 is often being used for market portfolio and also as a benchmark for beta stock in US. 
These explanation are the reason why S&P stock prediction is really important, especially for investors and stock trader to make a right investment decision.

## Algorithm Used in Code Documentation
In the proposal, Random Forest Tree is chosen as the algorithm for prediction model. 
This algorithm is one of machine learning method which works from the group of several decision tree.
Because the problem which will be resolved is a stock price prediction problem, Random Forest that will be used is Random Forest Regression.
In a standard tree, each node is split using split best among all variables, but in Random Forest, each node is divided using the best among a randomly selected subset of predictors at a node. 
Random Forest Regression builds a lot regression tree and will calculate the average value of the results prediction of response variables from all the regression trees.
Some advantages of Random Forest Algorithm are able to display low error, effective to estimate missing data, and able to cope large amounts of data training efficiently.

## Research Methodology
### 1. Business Understanding
1. **Date**:
Date is in YYYY-MM-DD format.
2. **Open**:
Share price at market opening. Price listed in USD.
3. **High**: 
The highest stock price reached on that date.  
4. **Low**: 
The lowest stock price reached on that date.  
5. **Close**: 
The last price that appears on a stock company before the stock exchange closes.
6. **Volume**:
Number of shares traded in a certain period of time and is located below stock price chart.
7. **Name**:
Name of the company that owns the shares listed on the S&P 500.

### 2. Data Understanding
This stage is the stage for understanding the data which has been obtained from the Kaggle website. 
At this stage, dataset will be modified, such as 'Name' column which only selecting data which comes from a company with the code 'AAPL' or Apple Inc in S&P 500. 
The ‘Date’ column will also be set, therefore it can be adjusted to the YYYY-MM-DD format. 
Besides that, there will be some visualizations and tables in the columns numerical, especially visualization of stock features displayed with the aim of understanding the contents of the data on the dataset better.
 
### 3. Data Preparation
This stage is the stage for preparing data before the data is modeled. 
Some action done before is to look at the density graph to see the distribution of numerical data, check for missing values in each column, and separate the features on the stock into independent variables (X-variable) and variables dependent (y-variable).
 
### 4. Modelling
The distribution of training and testing data is carried out using ratio 80:20. 
The training data size (X_train) is 1007 rows and 3 columns, while the size of the testing data (X_test) is 252 rows and 3 columns. 
Target data for training (y_train) has a size of 1007 rows, while the target data for testing (y_test) has a size of 252 rows.
Before performing hyperparameter tuning, the model Random Forest Regressor uses parameters n_estimators is 240, min_samples_leaf is 1, min_samples_split is 2, and bootstrap is True.

### 5. Modelling
To evaluate the regression problem, there are three methods that can be used for evaluate prediction models. 
These are Mean Absolute Error (MAE), R-squared, and Root Mean Squared Error (RMSE).

## Journal Link
Link: https://drive.google.com/file/d/1zQiM8LzaxrwKWgOvNtUfwhCffFhho2NX/view?usp=sharing
