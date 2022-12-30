# Credit_Risk_Analysis

## Analysis
I was tasked by Jill to carry out Credit card risk analysis using the data set provided in the LoanStats_2019Q1.csv file. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I was informed to employ different techniques to train and evaluate models with unbalanced classes. Jill also advised me to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduces bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results
After carrying out the analysis as mentioned above, the following observations are listed:

#### Random Over sampler

![RandomOverSampler](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler.jpg)

* After carrying out the analysis using RandomOversampler algorithm, we got the balanced accuracy of 0.646. High Risk Precision and recall values are 0.01 and 0.71 and 
  Low Risk precision and recall values are 1 and 0.58.  


#### SMOTE 

![SMOTE](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/SMOTE.jpg)

* After carrying out the analysis using SMOTE algorithm, we got the balanced accuracy of 0.659. High Risk Precision and recall values are 0.01 and 0.63 and 
  Low Risk precision and recall values are 1 and 0.68.  

#### Cluster Centroids

![CLusterCentroid](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids.jpg)

* After carrying out the analysis using Cluster Centroids algorithm, we got the balanced accuracy of 0.544. High Risk Precision and recall values are 0.01 and 0.69 and 
  Low Risk precision and recall values are 1 and 0.4.

#### SMOTEENN (Combination Sampling)

![SMOTEENN](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.jpg)

* After carrying out the analysis using SMOTEENN algorithm, we got the balanced accuracy of 0.666. High Risk Precision and recall values are 0.01   and 0.73 and Low     Risk precision and recall values are 1 and 0.6.

#### Balanced Random Forest Classifier

![BalancedRandomForest](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest.jpg)

* After carrying out the analysis using BalancedRandomForestClassifier algorithm, we got the balanced accuracy of 0.789. High Risk Precision and recall values are 0.03   and 0.7 and Low Risk precision and recall values are 1 and 0.87.

#### Easy Ensemble Classifier

![Easy Ensemble](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/EasyEnsemble.jpg)

* After carrying out the analysis using EasyEnsembleClassifier algorithm, we got the balanced accuracy of 0.932. High Risk Precision and recall values are 0.09   and 0.92 and Low Risk precision and recall values are 1 and 0.94.




## Summary

![Overall Analysis](https://github.com/Manishthapa2022/Credit_Risk_Analysis/blob/main/Images/Overall_data_summary.jpg)

In this project we evaluated a given dataset through six different models and came up with above analysis. The most important metrics here are the Precision, Sensitivity, and the f1 score. Although the High risk precision score for the six models was very low, it can be clearly seen that EasyEnsemble Classifier was the best performing model. When we compare the four models (i.e. RandomOverSample, SMOTE, ClusterCentroids, SMOTEENN) that resample the dataset, it can be seen that in this instance the SMOTEENN model was the best performing model with Highest accuracy acore(0.666) and overall high High and Low Risk Precision and recall numbers, although the Low Risk f1 factor for SMOTE(0.81) was slightly higher than the f1 factor for SMOTEENN(0.75).
Also, when SMOTEENN and BalancedRandomForest Classifier are compared, BalancedRandomForest classifier perofmred well with high overall numbers except for the High Risk Sensitivity matrics where SMOTEENN did marginally better. 
In conclusion, for this dataset, resampling did not considerably improve the performace metrics and BalancedRandomForest and EasyEnsemble Classifiers were the best performing models overall. 


#### Recommendation

With the given dataset, I would recommend to use the Easy Ensemble model, as it performs the best among the six machine learning models. It not only has a highest Balanced Accuracy score(0.932), but also the highest High Risk and Low Risk Precision, Recall and F1 scores. Although it can be seen that the High Risk Precision score (0.09) is quite low but in case of Credit Risk analysis, Recall/Sensitivity is more important as we want to ensure that no Actual High risk clients are treated as Low risk and the High Sensitivity score (0.92) ensures that this is the case. I would also suggest increasing the estimator values and trying this model to check if the performance metrics improves. 



