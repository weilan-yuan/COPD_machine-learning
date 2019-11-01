# COPD_machine-learning
Paper:"Development of a machine learning tool in the prediction of chronic obstructive pulmonary disease in Chinese population"
###
## python code 
1: data_clean.ipynb  
    Split <the 20191023_finalalldata.csv > to train data and test data  (train_data.csv & test_data.csv)   
2: copd_trainset_final_code.ipynb 
     Use the machine learning method(SVM，LogisticRegression，DecisionTree，MLP，Xgboost，KNN) with CV =5 to select the model and get average value of different evaluation parameter.The result are 5-fold tables, AUROC and PRROC with 5-fold labels, respectively. 

3: copd_validate_final_code.ipynb 
     Validate the 6 models(from the train data) in test_data and set the model parameter to get the best result. The result are tables, AUROC and PRROC,respectively. 
## data file  

4: data_1024  (input file)   
    the 20191023_finalalldata.csv

5: result_1024 (result file)  
    feature_importance (plot):only use the xgboost method to get the all feature importance.
    allfeature file: Result from above (2,3 code) include the 5 clinical features and 9 SNP OR values. 
    clinical file:  Result from above (2,3 code） just only include the 5 clinical feaures OR values.
    feature_snp file: Result from above (2,3 code) just only incule the 9 SNP OR values.
