# Credit_Risk_Analysis

## Overview 

In credit risk management, portfolio managers are interested to know which loan applications
are at high risk of default since such defaults are liable (liquidity loss) to the financial entity.
Supervised Machine learning (ML) as an explicit computer algorithm are used to solve such
classification problems. Credit risk is an inherently unbalanced classification problem, as good
loans outnumber risky loans.
The purpose of this analysis is to employ different ML techniques to train and evaluate models
with unbalanced classes to predict credit risk.

## Results 

Credit card dataset from LendingClub, a peer-to-peer lending services company was used for
this purpose. In all, six(6) ML techniques were used to train and evaluate using  balanced
accuracy scores, precision and recall scores. I obtained the following results:

- The RandomOverSampler algorithm using Logistic Regression Classifier showed a
balanced accuracy, precision and recall scores as 0.641, 0.99, 0.68 respectively.
![screenshot 1 here](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss1.png)


- The SMOTE algorithm using Logistic Regression Classifier showed a balanced accuracy,
precision and recall scores as 0.637, 0.99, 0.68 respectively. ![screenshot 2 here](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss2.png)


- The ClusterCentroid undersampling algorithm using Logistic Regression Classifier
showed a balanced accuracy, precision and recall scores as 0.529, 0.99, 0.45
respectively. ![screenshot 3 here](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss3.png)


- The SMOTEENN algorithm using Logistic Regression Classifier showed a balanced
accuracy, precision and recall scores as 0.624, 0.99, 0.55 respectively. ![screenshot 4
here](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss4.png)


- The Balanced Random Forest Classifier a typical ensemble tree based learners showed a
balanced accuracy score, precision score and recall scores as 0.7885, ![screenshot 5](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss5.png)

- The Easy Ensemble AdaBoost Classifier an ensemble of AdaBoost learners showed a
balanced accuracy, precision and recall scores as 0.932, 0.99, 0.94 respectively.
![screenshot 6 here](https://github.com/Elfreda2019/Credit_Risk_Analysis/blob/main/resources/ss6.png)


## Summary
From the presented results of the six(6) ML algorithms, the Easy Ensemble AdaBoost
Classifier which is an ensemble of AdaBoost learners trained on different balanced
boostrap samples shows good evaluation metrics among the other algorithms. Even
though the accuracy and recall scores are over 90% high for the minority class (high risk
group) and precision is low (0.09). I recommend the use of Easy Ensemble AdaBoost
Classifier to predict credit risk.
