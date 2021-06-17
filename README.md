# Predicting Impact on Readmission Rates for Patients Hospitalized with Diabetes

### Problem Statement 

During past decades, hospital readmissions have been the subject of retrospective surveys and prospective trials with a view to their prevention. Hospital readmission is when a discharged patient gets readmitted to a hospital within a certain period. The need for hospital readmission for certain conditions indicates hospital quality. Identifying patients at high risk early in hospitalization will help to reduce the readmission rate, in that hospitals can focus on preparing readmission for patients at high risk to shorten the length of readmission. 

### Goal of Analysis

The goal of the analysis is to find the determining factors that lead to higher readmission and correspondingly being able to predict which patients will get readmitted. Therefore, we proposed two research questions: 

1) What methods can we use to best predict hospital readmission in this dataset? 

2) What are the strongest predictors of hospital readmission in diabetic patients? 

### Method & Result 

We used Logistic Regression, Decision Tree, Random Forest, and XGboost classifiers to predict the readmission rate. Each algorithm was evaluated using 10-fold stratified cross-validation. All of our algorithms are evaluated using the area-under-the-curve (AUC), which is equivalent to the c-statistic in the binary classification scenario. In comparing of four models, it showed the XGBoost worked the best for predicting the admission rate, which achieves the highest accuracy as 0.94, with 0.61 on AUC, and the second-best model is Random Forest, which achieves 0.92 accuracy and 0.94 on AUC. In this study, we also identified the most important factors as the time_in_hospital and number of inpatient stays, number of diagnoses, which appears to associate with the severity of the disease. 

*This project serves for the final term requirement of DSC 462 data mining 2018 Fall course*

### Data Files

Data file: open the .csv file as running in the code in the jupyter notebook. Running the code step by step. 

The [data](https://drive.google.com/drive/folders/1kUA2g_5bJJRXGUCikCbdzNJ2gh0U-5Lu?usp=sharing) file includes three .csv file as follow: 

diabetic_data.csv 

modified_diabetes1205_beforeEDA.csv

smote_data.csv

### Summary of the Numerical Features

![Numerical_features](https://github.com/moggirain/Hospital_readmission_prediction/blob/master/Numerical_features.png)

 
### CONCLUSION
In this work we adopted machine learning methods to identify high risk patients and evaluated different machine learning algorithms. Compared to the previous analysis, our
study achieved high accuracy due to the sophisticated preprocessing procedure. The XGBoost method is reported to be the best method for prediction of the readmission rate for
diabetes patients.
We identified the most important factors as the time_in_hospital and number of inpatient, number of diagnosis, which appears to associate with the severity of the disease. Further studies could conduct more exploration when analyzing these factors individually. 
