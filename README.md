# SmartTarget_sales_prediction
The goal is to create a machine learning model that forecasts the chances of a client opting for the insurance. 

SmartTarget aims to predict customer conversion for an insurance company. Using historical data of the list of customers telecalled by the sales team of the insurance company, a machine learning model is developed that can identify which type of customers are more likely to avail of an insurance

The project aims to help the insurance company identify the customers that are most likely to convert, so that they can be targeted via call, and the cost of telephonic marketing campaigns can be reduced




## Project Approach

### 1. Importing and Installing Necessary Libraries
I have imported necessary libraries like numpy, pandas, sklearn, imblearn, seaborn, matplotlib, etc to use in the code block

### 2. Insights of the Data
I have loaded the dataset and converted it to a dataframe using pandas. After loading the data, I took insights of all the features and the target, and explained in detail about each feature

### 3. Generic Cleaning of Data
I have used functions like null_values, dtypes, and drop_duplicates to do general overall cleaning of the data

### 4. Column-Wise Cleaning 
For all the numeric features in the data, I've used the 'describe' function to view the summary statistics of the data. Outliers in the column are detected using the IQR approach, and then it is clipped to the q1 and q3 range  

For all the categorical features and the target, the unknown category of some of the features has been changed to the mode value of that feature

### 5. Final Checks
After cleaning all the features and target column-wise, once again, I have done the steps mentioned in the generic cleaning to ensure that well-cleaned data is used

### 6. Exploratory Data Analysis
The following data analysis has been done using seaborn and matplotlib

1. Countplot of the Distribution of Categorical Features in the Data
2. Boxplot of the Distribution of Continuous Features in the Data
3. Countplot of the Distribution of Target Variable in the Data
4. Feature v/s Target Plot for Categorical Columns
5. Feature v/s Target Plot for Continuous Columns


### 7. Encoding Categorical and Target Columns
All the categorical and target columns are label encoded


### 8. Splitting the Data
Using train_test_split from the model_selection package of the sklearn library, I have split the data into x_train, x_test, y_train, and y_test. 75% of the data goes to train, and 25% of the data goes to test

### 9. Balancing the Data
Using the  SMOTEENN technique from the imblearn library, I have balanced the data 

SMOTEENN combines SMOTE and Edited Nearest Neighbours(ENN) techniques. SMOTEENN performs undersampling and oversampling at the same time

### 10. Fit ML Models
I have used 6 classification models and trained the data. The 6 models are,

1. Logistic Regression
2. K-Nearest Neigbors
3. Decision Tree
4. Random Forest
5. Gradient Boosting
6. XGBoost


### 10.Model Evaluation
Generating a confusion matrix for each model and calculating the following Performance Parameters
1. Accuracy
2. Precision
3. Recall
4. F1 Score




