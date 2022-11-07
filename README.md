# Prudential_Insurance

### **Aim:**
Developing a predictive model that accurately classifies risk using a more automated approach.

### **Approach:**
In this approach along with Classification models, regression models are used with round up approach.

### Following steps have been performed:
1. Check for null values in the dataset
2. Since, few columns have high percentage of null values, columns with null percent greater than 40% have been removed.

images

3. Based on the skewness, rest of the columns are imputed using mean or median.
4. The dataset has only one categorical column [Product_Info_2] : Label Encoding
5. Remove outliers
6. Since the feature set is large and we cannot deduce the correlation we calculate feature score using Mutual independence Chi-square
7. Split data into X_train, y_train.
8. Models used:
&nbsp;&nbsp; - Classifier: Support Vector Machine, Logistic Regression
&nbsp;&nbsp; - Regressor: Linear Regressor, SGDRegressor
9. GridSearch: to crossvalidate the params within multiple models
