# Prediction-Analysis-of-high-risk-transactions
The project involves the prediction analysis of high risk transaction of metaverse transaction
## TITLE OF PROJECT
Prediction Analysis of a high risk financial transaction

### PROJECT OVERVIEW
This dataset contains blockchain financial transactions within the open metaverse aiming to provide a rich, diverse, and realistic set of data for developing anomaly, fraud analysis, and prescribe analytics in virtual environment 

### PROBLEM STATEMENT
Using Excel, how would you create a predictive model to identify transactions with a high risk score? Describe the steps you would take, including data preparation, model creation, and validation. What Excel functions or add-ins would you use?

### DATA SOURCE
[Metaverse Financial Transactions](https://t.co/MnIgCKQv0O)

### TOOL USED
Excel

### DATA CLEANING/PREPARATION
Missing values were checked for in the dataset. Excel's Filter feature was used to identify and filter out rows with missing data which there was none. Some columns, like transaction_type, location_region, ip_prefix, purchase_pattern, and age_group, are categorical and needed to be converted to numerical values. A mapping table was created to assign numerical values to each category.


### TYPE OF ANALYSIS
Regression Analysis

### DATA ANALYSIS
Excel Add Ins was installed in which there was now a data analysis space in the data tab. The risk was categorized into columns of high_risk, moderate_risk, and low_risk.

A conditional formatting was created so that where it is true for any of them, it returns 1 and returns 0 for false. The datasets was splitted into two parts: 89% was used for the training of the model, while the remaining 11% was used as the testing data. 

Regression analysis was chosen and the High_risk column was selected for the Input Y-range since we are looking to check for high risks only. Other columns(variables that could be responsible for high risk) which have been converted to numeric values were selected for the Input X-Range (ip_prefix, region, amount, age_group, transaction_patterns and the rest). 

After the output range has been chosen to display the regression results, the p-values of location, login_frequency, and session_duration turned out to be less than 0.05. The regression was done again excluding these 3 columns and the p-values were less than 0.05. The regression result was copied and pasted in the testing_data sheet were the calculations were done. 

### RESULTS
The values were checked if the approximate were the same as the high_risk values and it all turned out to be true after using the formula that goes thus: "coefficient of intercept + X1coefficient + X2coefficient + X3coefficient + X4coefficient + .... " where X1, X2, X3, X4,... represent the variables used for the comparisons in X-range. Since the values all turned out to be true, then the prediction analysis is valid.
