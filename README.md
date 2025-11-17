# Comparing-Classifiers in Bank-FDR-Subscription-Project
Prediction of whether a customer will Subscribe to Bank FDR or not

### Approach 
1. Read the file bank-additional-full.csv
2. Examine the data description from bank-additional-names.txt
3. There are several missing values in some categorical attributes, all coded with the "unknown" label. Treat the missing values using imputation techniques 
4. Encode and transform the features to prepare for machine learning 
5. Encode and transform target column y to prepare for machine learning
6. Identify correlation among features and target column y
7. Draw BOX plots for categorical columns
8. Draw Hist plots for Numerical columns
7. Perform descriptive and inferential statistics on the features 
9. Use T-test & Chi-square tests for identifying features that are significantly related to target variable column y 
10. Identify if the target variable y class imbalance is severe or not
11. Split data into Train and test set 
12. Goal is to predict if the client will subscribe target column y 
13. Build Logistic regression as baseline model using stratified k-fold cross-validation to get more stable estimates.
14. Perform the classification with k-nearest neighbors, decision trees, and support vector machines 
15. compare the performance with other the classifiers k-nearest neighbors, decision trees, and support vector machines using stratified k-fold cross-validation to get more stable estimates.

## EDA
CHARACTER COLUMNS
Admin, Retired, technician, Blue collar job customers are subscribed to a term deposit
Married people are more inclined to subscribe to a term deposit 
People with Degree are more inclined to subscribe to a term deposit 
People with No Loan are more inclined to subscribe to a term deposit 
Cellular is generally more favorable in terms of persuading customers to subscribing to a term deposit
Customers who have credit in default usually are not subscribed to a term deposit

NUMERICAL COLUMNS
The longer the duration to persuade a customer, the more likely it is for the customer to subscribe to a term deposit
Higher the Age, the more likely it is for the customer to subscribe to a term deposit

## Recommended Choice for Prediction:
K-Nearest Neighbors (KNN) is the most balanced classifier here, with:
High accuracy (90.4%) Best F1 for the minority class (0.54) Strong recall (0.49), meaning fewer false negatives.
