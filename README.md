# COPD_machine-learning
Paper:"Development of a machine learning tool in the prediction of chronic obstructive pulmonary disease in Chinese population"
###
## python code 
1: data_clean.ipynb  
    split <the 20191023_finalalldata.csv >   to train data and test data  (train_data.csv & test_data)   
2: copd_trainset_final_code.ipynb 
      use the machine learning method(SVM, LogisticRegression, DecisionTree,Nerualnetwork ,Xgboost ,KNN) with CV =5 to select the model and get
  mean value of different evaluation parameter.The result is 5fold table and AUROC and PRRUC with 5fold label 

3:copd_validate_final_code.ipynb 
     test the 6 models(from the train data) in test_data (set the model parameter). The result is table and AUROC and PRRUC  
#### data file  
data_1024  (input file )
result_1024( result file) 
4: feature_importance 
   only use the xgboost method to get the all feature importance 
   
5: allfeature  file : Result from above (2,3 code )include the 5 clinical features and 9 SNP OR values 
   clinical file  : Result from above (2,3 code ) just only include the 5 clinical feaures
   feature_snp file : Result from above (2,3 code ) just only incule the 9 SNP OR values 
