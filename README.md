# Prudential_Insurance

![alt-text](https://github.com/HitPant/Insurance_Risk_Prediction/blob/main/images/insurance.jpg)

## **Problem Statement:**
Predict customer risk based on the input parameters.<br>
Risk can be in range 1-8.<br>
1 is lowest and 8 is the highest risk.<br>

## **Aim:**
Developing a predictive model that accurately classifies risk using a more automated approach.

## **Approach:**
In this approach along with Classification models, regression models are used with round up approach.

### Following steps have been performed:
1. Check for null values in the dataset
2. Since, few columns have high percentage of null values, columns with null percent greater than 40% have been removed.

![alt-text](https://github.com/HitPant/Prudential_Insurance/blob/main/images/missratio.jpg)

3. Based on the **skewness**, rest of the columns are imputed using mean or median.
4. The dataset has only one categorical column [Product_Info_2] : Label Encoding
5. **Remove outliers**
6. Since the feature set is large and we cannot deduce the correlation we calculate feature score using Mutual independence Chi-square

![alt-text](https://github.com/HitPant/Prudential_Insurance/blob/main/images/chi.jpg)

7. **Split data** into X_train, y_train.
8. **Models used**:<br>
&nbsp;&nbsp; - **Classifier**: Support Vector Machine, Logistic Regression<br>
&nbsp;&nbsp; - **Regressor**: Linear Regressor, SGDRegressor<br>
&nbsp;&nbsp; - **Anomaly detection**: Isolation forest
9. **GridSearch**: to crossvalidate the params within multiple models
10. Anomaly detection using Isolation forest

## Model Comparision
![alt-text](https://github.com/HitPant/Prudential_Insurance/blob/main/images/cmp.jpg)
