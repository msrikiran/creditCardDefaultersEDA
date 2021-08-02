# creditCardDefaultersEDA

# Problem Statement

To build a classification methodology to determine whether  a Person defaults the credit card payment for the next month.

### Data Description:

The data has been extracted from the census bureau.

The data contains 32561 instances with the following attributes:



##### Features:

1.	**LIMIT_BAL**: continuous. Credit Limit of the person.
2.	**SEX**: Categorical: 1 = male; 2 = female
3.	**EDUCATION**: Categorical: 1 = graduate school; 2 = university; 3 = high school; 4 = others
4.	**MARRIAGE**: 1 = married; 2 = single; 3 = others
5.	**AGE**: num: continuous. 
6.	**PAY_0 to PAY_6:** History of past payment. We tracked the past monthly payment records (from April to September, 2005)
7.	**BILL_AMT1 to BILL_AMT6:** Amount of bill statements.
8.	**PAY_AMT1 to PAY_AMT6:** Amount of previous payments. 

##### Target Label:

Whether a person shall default in the credit card payment or not.

9.	**default payment next month:**  Yes = 1, No = 0.

### Steps for Model Training

1. START

2. Read the file

3. Data Preprocessing

   a. Check for null values in the columns. If present, impute the null values using the categorical imputer.(The **CategoricalImputer()** replaces missing data in categorical variables by an arbitrary value or by the most frequent category.)

   b. Scale the numerical values using the Standard Scaler.

   (**StandradSclaer:** When need to transform a feature so it is close to normal distributed, StandardScaler standardizes a feature by removing the mean and dividing each value by the standard deviation.

   It results a distribution with a standard deviation equal to 1 (and variance equal to 1 ). If you have outliers in your feature(column). normalizing your data will scale most of the data to a small interval  )

   c. Check for Correlation.( **corr() **is used to find the pairwise correlation of all columns in the dataframe. Any `na` values are automatically excluded. For any non-numeric data type columns in the dataframe it is ignored.)

   

4. Data Visualization

5. Apply Algorithms

6. Hyper parameter tuning

7. Get the best model

8. export to CSV

9. END
