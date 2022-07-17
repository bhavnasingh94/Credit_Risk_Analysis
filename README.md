# Credit_Risk_Analysis_MachineLearning

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. 

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the **_RandomOverSampler_** and **_SMOTE_** algorithms, and undersample the data using the **_ClusterCentroids_** algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, **_BalancedRandomForestClassifier_** and **_EasyEnsembleClassifier_**, to predict credit risk.

## Results

The LendingClub database contained 115,675 loan applications in the first quarter of 2019. This loan status was to determine if the applicants are considered a low or high risk. According to the data, 68,470 of the applicants were considered low-risk, while 347 were high-risk.

![Low HighRisk](https://user-images.githubusercontent.com/98790082/179389223-f73a5485-ed57-4e96-aa8f-3a706771b347.png)


Below are the Precision Scores (**_pre_**) for predicting high risk, Recall Score (**rec**) for predicting high-risks, and Balanced Accuracy (**_geo_**) for predicting high-risk.

## Random Oversampling

The precision score for predicting the high risk applications was 0.01. The balanced accuracy was 0.65 and recall score for predicting high-risk's was 0.72.

![RandomOverSampling](https://user-images.githubusercontent.com/98790082/179389292-ab34df4c-3631-4ef1-88af-56da172cc01e.png)


## Cluster Centroids

![ClusterCentroids](https://user-images.githubusercontent.com/98790082/179389316-cb4f160f-6227-4d66-815d-c5a306b72c42.png)

## SMOTE 

![SMOTE](https://user-images.githubusercontent.com/98790082/179389326-31130502-a15c-49f0-9924-d0dd068cee89.png)

## SMOTTEEN

![SMOTTEEN](https://user-images.githubusercontent.com/98790082/179389335-addcd005-9a55-48ae-ac08-4d7c1e0c5255.png)

## Easy Ensemble Classier

![EasyEnsemble](https://user-images.githubusercontent.com/98790082/179389498-811eb5da-8b83-4947-b4f5-a2eb56d0be69.png)


## Summary 

Of all the Machine Learning models, EasyEnsembleClassifier model proved to be more accurate; yielding highest accuracy rate of 93% with a rate of precision of predicting high and low risk applications at 9% and 100%, respectively. This models precision score was 0.09 (9%), which is higher than other 5 models tested. This means that the loans flagged as "high-risk" have only 9% likelihood of actually being high risk. In the future, I would recommend continuing to build and evaluated more models using other algorithms and features. If no other model can improve the performance of the current Easy Ensemble Classifier, then I would continue to utilize it for predicting credit risk until something better comes up as this seems to be best working algorithm for predicting high-risk applications as of now.
