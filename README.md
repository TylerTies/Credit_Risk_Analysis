# Credit Risk Analysis
## Overview
Credit risk is an unbalanced classification problem.  In this project I used a credit card dataset from LendingClub.  I analyzed six different algorithms with the imbalanced-learn and scikit-learn libraries to determine which would be most appropriate for determining credit risk.

## Results

- **Naive Random Oversampling**
    - Accuracy: 62.9%
    - Precision: 0.01
    - Recall: 0.57
![Naive Random Oversampling](/Resources/naive_random_oversampling.png)

- **SMOTE Oversampling**
    - Accuracy: 62.8%
    - Precision: 0.01
    - Recall: 0.62
![SMOTE Oversampling](/Resources/smote_oversampling.png)

- **Cluster Centroids**
    - Accuracy: 51.6%
    - Precision: 0.01
    - Recall: 0.60
![Cluster Centroids](/Resources/cluster_centroids.png)

- **SMOTEENN**
    - Accuracy: 64.1%
    - Precision: 0.01
    - Recall: 0.70
![Naive Random Oversampling](/Resources/smoteenn.png)

- **Random Forest**
    - Accuracy: 67.2%
    - Precision: 0.73
    - Recall: 0.34
![Random Forest](/Resources/random_forest.png)

- **Easy Ensemble**
    - Accuracy: 92.5%
    - Precision: 0.07
    - Recall: 0.91
![Easy Ensemble](/Resources/easy_ensemble.png)


## Summary
The random forest algorithm produced the best f1 scores at 0.47, which balances sensitivity and precision. This would mean the random forest method is best for generally predicting the credit risk. However, the accuracy isn't ideal.  Accuracy is higher for the easy ensemble algorithm. If the company was wanting to make sure to identify all high credit risk, they should chose this algorithm. The downside is they will have more work sifting through low credit risk customers who were falsely identified as high risk. The precision of this model is very low. If that additional work is acceptable, the company should chose the easy ensemble model.