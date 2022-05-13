# Random_Forest_Excersie 
The pre-trained models can be found here:
https://drive.google.com/drive/folders/1gGdaEMenUj5yVl-WLW7qSm29x63x1VGK?usp=sharing



This the performance metrics for the model: random_forest_n_estimtor_100.joblib

for 80: 20 split of the data for training and testing.

For the following Parameters in use:

{'bootstrap': True,
 'ccp_alpha': 0.0,
 'class_weight': None,
 'criterion': 'gini',
 'max_depth': None,
 'max_features': 'auto',
 'max_leaf_nodes': None,
 'max_samples': None,
 'min_impurity_decrease': 0.0,
 'min_impurity_split': None,
 'min_samples_leaf': 1,
 'min_samples_split': 2,
 'min_weight_fraction_leaf': 0.0,
 'n_estimators': 100,
 'n_jobs': None,
 'oob_score': False,
 'random_state': 42,
 'verbose': 0,
 'warm_start': False}
 
 -------------------------TEST SCORES-----------------------
 
Recall: 23.1476

Precision: 86.3014

F1-Score: 36.5041

Accuracy score: 81.3122

AUC Score: 61.0186


 
This the performance metrics for the model: random_forest_n_estimtor_1000.joblib 

for 80: 20 split of the data for training and testing.

For the following Parameters in use: 

{'bootstrap': True,
 'ccp_alpha': 0.0,
 'class_weight': None,
 'criterion': 'gini',
 'max_depth': None,
 'max_features': 'auto',
 'max_leaf_nodes': None,
 'max_samples': None,
 'min_impurity_decrease': 0.0,
 'min_impurity_split': None,
 'min_samples_leaf': 1,
 'min_samples_split': 2,
 'min_weight_fraction_leaf': 0.0,
 'n_estimators': 1000,
 'n_jobs': None,
 'oob_score': False,
 'random_state': 42,
 'verbose': 0,
 'warm_start': False}
 
 -------------------------TEST SCORES-----------------------
 

Recall: 22.7189

Precision: 89.6857

F1-Score: 36.2541

Accuracy score: 81.459

AUC Score: 60.9647



This the performance metrics for the model: random_forest_rf_clf.joblib 

for 80: 20 split of the data for training and testing.

For the following Parameters in use: 

{'bootstrap': True,
 'ccp_alpha': 0.0,
 'class_weight': None,
 'criterion': 'gini',
 'max_depth': None,
 'max_features': 'auto',
 'max_leaf_nodes': None,
 'max_samples': None,
 'min_impurity_decrease': 0.0,
 'min_impurity_split': None,
 'min_samples_leaf': 1,
 'min_samples_split': 2,
 'min_weight_fraction_leaf': 0.0,
 'n_estimators': 100,
 'n_jobs': None,
 'oob_score': False,
 'random_state': 100,
 'verbose': 0,
 'warm_start': False}

-------------------------TEST SCORES-----------------------

Recall: 36.9259

Precision: 58.3925

F1-Score: 45.242

Accuracy score: 79.2563

AUC Score: 64.4873



# Data Preprocessing:
 There are several missing values in the following features
 Credit Score                   ---  20553 missing values
 Years in current job           ---  4511 missing values
 Annual Income                  ---  20553 missing values
 Months since last delinquent   ---   56662 missing values
 Since the count of each one of the features that have null
 vlaues or missing values  is less than %50 of the data size (105549)
 we can fill the null values with the mean value from the feature


 Encoding of Categorical features:
 “years_in_current_job” we just trim 
 the ‘year’ part and leave the years only

# Plot the Feature importance with scroes
![image](https://user-images.githubusercontent.com/105464639/168318536-47ee8935-9b56-4f64-ae4c-cd9cee736c08.png)

 The feature "Credit Score" has the longest bar 
 that shows it is the most important feature in case 
 of "Loan Status" or "defaults"
 The next features that are also important are in this order:
 2 - 'Current Loan Amount'
 3 - 'Maximum Open Credit'
 4 - 'Current Credit Balance'
 
 The least important fearures are 'Home Wownership' and 'Purpose'
