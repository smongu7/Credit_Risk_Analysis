# Credit_Risk_Analysis
## Overview
The purpose of this analysis was to introduce us to supervised machine learning by applying it to predicting credit risk. In the process of doing so, we learned how to:
- explain how a machine learning algorithm is used in data analytics.
- create training and test groups.
- implement logistic regression, decision trees, random forest, and support vector machine algorithms.
- interpret results of logistic regression, decision trees, random forest, and support vector machine algorithms.
- compare the advantages and disadvantages of each learning algorithm.
- determine which learning algorithm is best used for a given data set.
- use ensemble and resampling techniques to improve model performance.
## Results:
#### Naive random oversampling
![random-over](https://user-images.githubusercontent.com/94420548/164778224-1839db93-3814-40f9-a8e2-1f38a2958307.png)

- The balanced accuracy score of this algorithm was about 62.8%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 68%.
#### SMOTE oversampling
![smote-over](https://user-images.githubusercontent.com/94420548/164778244-f375989b-049c-4a88-98ea-34bad7c30e35.png)

- The balanced accuracy score of this algorithm was about 62.8%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 63%.
#### Undersampling
![under](https://user-images.githubusercontent.com/94420548/164778264-5722cb70-3537-4e56-b8c9-b0a93ccd23ac.png)

- The balanced accuracy score of this algorithm was about 53.0%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 45%.
#### Combination (SMOTEENN)
![combo](https://user-images.githubusercontent.com/94420548/164778298-170937a3-899d-4cd8-8020-9caac09e8abd.png)

- The balanced accuracy score of this algorithm was about 64.1%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 58%.
#### Balanced Random Forest Classifier
![forest](https://user-images.githubusercontent.com/94420548/164778339-1362ac51-a83a-4332-8233-5743ec3d78b8.png)

- The balanced accuracy score of this algorithm was about 78.8%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 91%.
#### EasyEnsemble Adaboost
![adaboost](https://user-images.githubusercontent.com/94420548/164778385-e994c8d1-c87e-48e2-b518-05c1f8d84cfc.png)

- The balanced accuracy score of this algorithm was about 92.5%.
- The overall precision score of this algorithm was 99%.
- The recall score of this algorithm was 94%.
## Summary:
The overall precision scores of all 6 algorithms were virtually identical being 99% overall for every one. The balanced accuracy score for naive random oversampling, SMOTE oversampling and SMOTEENN sampling were quite low, being 64.1% at best and 53.0% at worst. The balanced accuracy score went up in the balanced random forest classifier to 78.8%, and jumped to 92.5% with the easyensemble adaboost algorithm. The recall score was also quite low for the naive random oversampling, SMOTE oversampling, undersampling and SMOTEENN algorithms, being 45% at worst and 68% at best. The recall score was relatively high with the balanced random forest classifier at 91% and even higher with the adaboost algorithm at 94%. This is a significant improvement on the first 4 algorithms, however there is one more factor to consider; the precision scores on high risk loans for every algorithm is exceedingly low. Even on the best algorithm of the six, the precision score for high risk loans is still under 10%. I would recommend further improving the algorithm to increase accuracy and lower the risk of approving high-risk loans.
