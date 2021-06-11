# LENDING CLUB CEDIT RISK ANALYSIS

## Overview of Risk Analysis:
 The purppose of our analysis is to apply machine learning to solve credit card risk from the LendingClub dataset.  I will be using several different 
 techniques to train and evaluate models amongst the unbalanced classes.

## RESULTS:

### Random Over Sampler Method

![RandomAccuracy](https://user-images.githubusercontent.com/71041680/121614183-2a2e9600-ca2c-11eb-9053-a248095904da.png)

![RandomMatrix](https://user-images.githubusercontent.com/71041680/121614190-2d298680-ca2c-11eb-95f9-1797836fc342.png)

- Balanced Accuracy Score: 65%
- Precison High Risk: 1%
- Precision Low Risk: 100%
- Recall High risk: 69%
- Recall Low risk: 60%


### SMOTE Oversample Method

![SMOTEAccuracy](https://user-images.githubusercontent.com/71041680/121614201-30247700-ca2c-11eb-9207-d71ac76fb512.png)

![SMOTEMatrix](https://user-images.githubusercontent.com/71041680/121614208-33b7fe00-ca2c-11eb-8845-266a6b3f9f85.png)

- Balanced Accuracy Score: 67%
- Precison High Risk: 1%
- Precision Low Risk: 100%
- Recall High risk: 71%
- Recall Low risk: 63%


### Cluster Centroids Sample Method

![ClusterAccuracy](https://user-images.githubusercontent.com/71041680/121615428-da050300-ca2e-11eb-88ef-7473af819e4c.png)

![ClusterMatrix](https://user-images.githubusercontent.com/71041680/121615430-dbcec680-ca2e-11eb-89f2-3266f12af611.png)

- Balanced Accuracy Score: 58%
- Precison High Risk: 1%
- Precision Low Risk: 100%
- Recall High risk: 71%
- Recall Low risk: 45%

### SMOTEEN Sample Method

![SMOTEENAccuracy](https://user-images.githubusercontent.com/71041680/121614223-3b77a280-ca2c-11eb-9407-caa32dd4baf9.png)

![SMOTEENMatrix](https://user-images.githubusercontent.com/71041680/121614229-3dd9fc80-ca2c-11eb-9811-071f0b0004ed.png)

- Balanced Accuracy Score: 67%
- Precison High Risk: 1%
- Precision Low Risk: 100%
- Recall High risk: 72%
- Recall Low risk: 61%

### Balanced Random Forest Classifier Method

![BalanceRandomAccuracy](https://user-images.githubusercontent.com/71041680/121614313-6a8e1400-ca2c-11eb-862c-476dbec82f6d.png)

![BalancedRandomMatrix](https://user-images.githubusercontent.com/71041680/121614320-6d890480-ca2c-11eb-85a9-05d40d277883.png)

- Balanced Accuracy Score: 65%
- Precison High Risk: 56%
- Precision Low Risk: 100%
- Recall High risk: 30%
- Recall Low risk: 100%

### Easy Ensemble AdaBoost Classifier Method

![EEAccuracy](https://user-images.githubusercontent.com/71041680/121614337-72e64f00-ca2c-11eb-944b-07c99d8a93ba.png)

![EEMatrix](https://user-images.githubusercontent.com/71041680/121614348-7548a900-ca2c-11eb-8a89-b07fd5a2803c.png)

- Balanced Accuracy Score: 92%
- Precison High Risk: 6%
- Precision Low Risk: 100%
- Recall High risk: 91%
- Recall Low risk: 94%
- 
## SUMMARY:
- 4 of the 6 models performed equally with regard to high and low risk precision.  The Easy Ensemble performed slightly better in the precision high risk, returning a rate of 6   6% and the balanced random performed significantly better with 56% (all models returned 100% with low risk precision).  
- It was Easy Ensemble method with the overall best performance, with a significantly higher balanced accuracy rate (92%) than the other models.  Additionally the recall for     both high and low risk overall performed much better than the other models.  It would be myh recommendation to utilize the Easy Ensemble Adaboost Classifier method
  for analysis of this dataset.
