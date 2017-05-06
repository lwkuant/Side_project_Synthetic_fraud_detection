# Side Project: Synthetic Fraud Detection

## Overview
The goal of this peoject is to identify the fraudulent transactions.

Since this dataset is very imbalanced, it can simulate the problems we face in reality.

The best performaing model so far in this task is xgboost model.
<br/>

#### The performance of the final model:

<img src="https://github.com/lwkuant/Side_project_Synthetic_fraud_detection/blob/master/average_model.png">
<br/>

#### Here are the conclusions and takeaways:

1. I use feature transformation (log transformation) to get better features.

2. After removing highly-correlated features, the model performs better.

3. I find that using different thresholds would yield significantly different performances on precision, recall and f1-score on similar models with slightly different hyperparameters. In reality, we have to consider the goals of this task to get the optimal results.

4. Slightly different settings of hyperparameters on xbgoost model (n_estimators, learning_rate and max_depth) can have quite different results, which is very worth further studying.

5. Random forest model is likely to have better result since it has similar performance with xgboost model when modeling the training set; however, the memory limitation on my computer stops me from trying that.

6. Imbalanced dataset is still a hard task to handle, which requires more trying besides undersampling.

7. Further work:
    * More feature engineering
    * Try more different ways to deal with imbalanced data
    * Try ensemble model techniques like stacking
<br/>

#### The related information regarding this dataset can be accessed below:

* [kaggle (the data source)](https://www.kaggle.com/ntnu-testimon/paysim1)

## Notice
Link to the work [here](https://github.com/lwkuant/Side_project_Synthetic_fraud_detection/blob/master/Synthetic_fraud_detection.ipynb)