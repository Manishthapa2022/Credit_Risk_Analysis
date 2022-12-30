# Credit_Risk_Analysis

## Analysis
I have been tasked by Jill to carry out Credit card risk analysis using the data set provided in the LoanStats_2019Q1.csv file. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I have been informed to employ different techniques to train and evaluate models with unbalanced classes. Jill has advised me to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, I will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
After carrying out the analysis as mentioned above, the following observations are listed:

#### Random Over sampler

![RandomOverSampler](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/Oversampling.png)

* After carrying out the analysis using RandomOversampler algorithm, we got the balanced accuracy of 0.646. High Risk Precision and recall values are 0.01 and 0.71 and 
  Low Risk precision and recall values are 1 and 0.58.  


#### SMOTE 

![SMOTE](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/SMOTE.png)

* After carrying out the analysis using SMOTE algorithm, we got the balanced accuracy of 0.659. High Risk Precision and recall values are 0.01 and 0.63 and 
  Low Risk precision and recall values are 1 and 0.68.  

#### Cluster Centroids

![CLusterCentroid](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/ClusterCentrids.png)

* After carrying out the analysis using Cluster Centroids algorithm, we got the balanced accuracy of 0.544. High Risk Precision and recall values are 0.01 and 0.69 and 
  Low Risk precision and recall values are 1 and 0.4.

#### SMOTEENN (Combination Sampling)

![SMOTEENN](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/SMOTTENN.png)

* After carrying out the analysis using SMOTEENN algorithm, we got the balanced accuracy of 0.666. High Risk Precision and recall values are 0.01   and 0.73 and Low     Risk precision and recall values are 1 and 0.6.

#### Balanced Random Forest Classifier

![BalancedRandomForest](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/Random_rain_forest.png)

* After carrying out the analysis using BalancedRandomForestClassifier algorithm, we got the balanced accuracy of 0.789. High Risk Precision and recall values are 0.03   and 0.7 and Low Risk precision and recall values are 1 and 0.87.

#### Easy Ensemble Classifier

![Easy Ensemble](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/Easy_ensemble.png)


* After carrying out the analysis using EasyEnsembleClassifier algorithm, we got the balanced accuracy of 0.932. High Risk Precision and recall values are 0.09   and 0.92 and Low Risk precision and recall values are 1 and 0.94.




## Summary

![Overall Analysis](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/Overall_data_summary.png)



