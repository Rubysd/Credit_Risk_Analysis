# Credit_Risk_Analysis

![image](https://user-images.githubusercontent.com/86340630/138366118-6374d28a-8258-4d84-b7e7-2870cac6575e.png)

## Overview of Project

Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

Deliverables:
This new assignment consists of three technical analysis deliverables and a written report.

### Deliverable 1: Use Resampling Models to Predict Credit Risk
### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
### Deliverable 4: A Written Report on the Credit Risk Analysis README.md

# Deliverable 1:

### Use Resampling Models to Predict Credit Risk

### Deliverable Requirements:

Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

To Deliver.

Follow the instructions below:

Follow the instructions below and use the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 1.

Open the credit_risk_resampling_starter_code.ipynb file, rename it credit_risk_resampling.ipynb, and save it to your Credit_Risk_Analysis folder.

Using the information we’ve provided in the starter code, create your training and target variables by completing the following steps:

* Create the training variables by converting the string values into numerical ones using the get_dummies() method.
* Create the target variables.
* Check the balance of the target variables.

Next, begin resampling the training data. First, use the oversampling RandomOverSampler and SMOTE algorithms to resample the data, then use the undersampling ClusterCentroids algorithm to resample the data. For each resampling algorithm, do the following:

* Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
* Calculate the accuracy score of the model.
* Generate a confusion matrix.
*Print out the imbalanced classification report.

Save your credit_risk_resampling.ipynb file to your Credit_Risk_Analysis folder.

#### Deliverable 1 Requirements

For all three algorithms, the following have been completed:

* An accuracy score for the model is calculated
* A confusion matrix has been generated
* An imbalanced classification report has been generated

# Deliverable 2:

### Use the SMOTEENN algorithm to Predict Credit Risk

### Deliverable Requirements:

Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll use a combinatorial approach of over and undersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

To Deliver.

Follow the instructions below:

Follow the instructions below and use the information in the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 2.

1. Continue using your credit_risk_resampling.ipynb file where you have already created your training and target variables.
2. Using the information we have provided in the starter code, resample the training data using the SMOTEENN algorithm.
3. After the data is resampled, use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
4. Calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
 
 Save your credit_risk_resampling.ipynb file to your Credit_Risk_Analysis folder.

### Deliverable 2 Requirements

The combinatorial SMOTEENN algorithm does the following:

* An accuracy score for the model is calculated
* A confusion matrix has been generated
* An imbalanced classification report has been generated

# Deliverable 3:

### Use Ensemble Classifiers to Predict Credit Risk
### Deliverable Requirements:

Using your knowledge of the imblearn.ensemble library, you’ll train and compare two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. Using both algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

To Deliver.

Follow the instructions below:

Follow the instructions below and use the information in the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 3.

1. Open the credit_risk_ensemble_starter_code.ipynb file, rename it credit_risk_ensemble.ipynb, and save it to your Credit_Risk_Analysis folder.

2. Using the information we have provided in the starter code, create your training and target variables by completing the following:
   * Create the training variables by converting the string values into numerical ones using the get_dummies() method.
   * Create the target variables.
   * Check the balance of the target variables.

3. Resample the training data using the BalancedRandomForestClassifier algorithm with 100 estimators.
   * Consult the following Random Forest documentation for an example.
4. After the data is resampled, use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
5. Calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
6. Print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
7. Next, resample the training data using the EasyEnsembleClassifier algorithm with 100 estimators.
   * Consult the following Easy Ensemble documentation for an example.
8. After the data is resampled, use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
9. Calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.

Save your credit_risk_ensemble.ipynb file to your Credit_Risk_Analysis folder.

### Deliverable 3 Requirements

The BalancedRandomForestClassifier algorithm does the following:

* An accuracy score for the model is calculated
* A confusion matrix has been generated
* An imbalanced classification report has been generated
* The features are sorted in descending order by feature importance

The EasyEnsembleClassifier algorithm does the following:

* An accuracy score of the model is calculated
* A confusion matrix has been generated
* An imbalanced classification report has been generated

### DELIVERABLE RESULTS:

Below are the results from the various techniques used to predictive model for High-Risk loans.

### Oversampling

Using oversampling, it can be observed that the high risk precision is 1%, its recall is 69%, while the low risk has a 100% precision but the recall has 59% of accuracy.

![Captura de pantalla (941)](https://user-images.githubusercontent.com/86340630/138388760-34e3e71c-a492-4957-acb6-815b05e39741.png)

### SMOTE oversampling

With SMOTE oversampling, the high risk precision is 1% and the recall is 63%. The low risk has a precision of 100% while the recall is 69%.

![Captura de pantalla (943)](https://user-images.githubusercontent.com/86340630/138389366-21c5a034-e8d3-473a-a105-473110f21236.png)

### Undersampling

Undersampling presents an accuracy in high risk precision of 1% and a recall of 69%. The low risk presents a precision of 100% and a recall of 40%.

![Captura de pantalla (945)](https://user-images.githubusercontent.com/86340630/138389718-af9f19c9-a160-4351-a1a4-1d52cd30cbdb.png)

### Combination sampling

Combination sampling (under and oversampling), high risk precision has a percentage of 1% and the recall 72%. The low risk presents a precision of 100% but the recall is 57%.

![Captura de pantalla (947)](https://user-images.githubusercontent.com/86340630/138390074-1d4d74ef-4c59-480f-8ff1-7acacb42766b.png)

### Balanced random forest

Balanced ramdom forest, presents a high risk precision of 3% and a recall of 67%. The low risk has a precision of 100% and a recall of 87%. In this case, the high risk precision improved a bit.

![Captura de pantalla (949)](https://user-images.githubusercontent.com/86340630/138390856-344a14c4-1257-4f86-a659-d217dfaf272e.png)

### AdaBoost

AdaBoost, has a high risk precision of 9% and a recall of 92%, it also has a low risk of 100% and a recall of 94%.

![Captura de pantalla (951)](https://user-images.githubusercontent.com/86340630/138391259-bd703aad-d384-4745-8565-66e193b1318e.png)

### Summary:

With the results obtained, using F1 as a metric, and considering the respective precision and recovery, the best models were Balanced Random Forests and AdaBoost. Even if those models were the ones with significant precision, none of the models should be used to predict high risks due to low precision in the respective risk percentage.







