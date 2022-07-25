# Credit_Risk_Analysis

## Overview of the analysis: 

This analysis attempts to predict credit risk by using Machine Learning statistical algorithms to make predictions based on data patterns. Supervised Learning where the data includes a labeled outcome is used.

Different Machine Learning techniques are used to train and evaluate the data with unbalanced classes. Dataset from the LendingClub has an unbalanced classification problem since the number of good loans is far more thhan those of risky loans. To balance out the classifications to to have better predictions and accuracy score we apply different Machine Learning algorithms to resample the data. The algorithms included RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.

## Results: 

- Naive Random Oversampling results: Our balanced accuracy test it 62%, the precision for the high_risk has a very low positivity at 1% and the recall is 60%
![IMAGE_DESCRIPTION](/Images/naive.png)

- SMOTE oversampling results: the accuracy score is 65%, the precision for the high_risk loans has a low positvity again at 1% and recall is 64% overall
![IMAGE_DESCRIPTION](/Images/under.png)

- Undersampling results: balanced accuracy score is 51% overall, the precision is at 99% and the recall is 59%
![IMAGE_DESCRIPTION](/Images/smote.png)

- Combination(over and undersampling) results: balanced accuracy score is 64% the precision is 99% and the recall is 57% overall
![IMAGE_DESCRIPTION](/Images/mixed.png)

- Balanced Random Forest Classifier results: the accuracy score is 79% the overall precision is 99% and the recall is 87%
![IMAGE_DESCRIPTION](/Images/forest.png)

- Easy Ensemble AdaBoost Classifier results: the accuracy score is 92.5 the precision is 99% and the recall is 94%
![IMAGE_DESCRIPTION](/Images/ensemble.png)

## Summary: 

- The first four models where we undersampled, oversampled or did a combination of the two, the accuracy score was not good (50s-60s) and the recall was also low.
- The two ensemble models had a much better accuracy score with 79% for the Balanced Random Forest and 92.5% for the Easy Ensamble. The recall was also improved bweing much higher than that of the four earlier models.
- All six models had very low precision which means low reliability that those identified as high-risk, were actually high risk. 
- If a company has to choose between these models I will recommend the Easy Ensemble model since it had the best overall accurancy score and best balance between sensitivity and precision. However if time and resources are available to create and test other models I would recommend that and not using any oif these 6 models.
