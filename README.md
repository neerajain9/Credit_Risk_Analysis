# Credit Risk Analysis (Module 17 Challenge)

## Overview
Jill has put all the faith in us and given us an opportunity to help her analyze a real-world challenge; Credit Risk Analysis.

In usual the good loans outnumber the bad loans. So, this challenge is an inherently unbalanced classification issue. With such a disparity in the classes, the normal predictions will favor good loans prediction only. We need to find ways to overcome this problem.

So, we will deploy different techniques to train and evaluate models with unbalanced classes. We will oversample, undersample, and combinatorial approaches to resample the data. We will then, to reduce bias, compare the two machine learning models; BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Based on the performance of each model we will cast our recommendations.

## Results

### Oversampling
#
#### 1. Random Oversampling
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/RandomOversampling_balanced%20Accuracy%20score.png)

Random oversampling has about 61.9% accuracy score. This means the model generated 61.9% of the predictions correct.

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/RandomOversampling_balanced%20Accuracy%20score.png?raw=true)

[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/RandomOversampling_classification%20report.png)
#
**Here,** 

**'0' represents 'bad credit"**

**'1' represents 'good credit'**

**NOTE: This representation is consistent in all the following model analysis**

#
**The precision** in predicting "bad credit" is 1 % with the prediction of 100% "good credit". This represents inherently unbalanced classification issue that we are analysing here. This measure is not of use in our analysis.

**The recall (sensitivity)** in predicting "bad credit is 66% where the "good credit" prediction is 57%. Overall, the model predicted 58% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/RandomOversampling_classification%20report.png?raw=true)

#
#### 2. SMOTE Oversampling
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/SMOTE%20Oversampling_balanced%20Accuracy%20score.png)

SMOTE oversampling has about 63.9% accuracy score. This means the model generated 63.9% of the predictions correct.

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/SMOTE%20Oversampling_balanced%20Accuracy%20score.png?raw=true)


[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/SMOTE%20Oversampling_classification%20report.png)


**The precision** 
This measure is not of use in our analysis due to biases as explained above.

**The recall (sensitivity)** in predicting "bad credit is 63% where the "good credit" prediction is 65%. Overall, the model predicted 65% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/SMOTE%20Oversampling_classification%20report.png?raw=true)

#
### Undersampling
#
#### 3. Undersampling
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/UnderSampling_balanced%20Accuracy%20score.png)

Undersampling suggests 50.6% accuracy score. This means the model generated 50.6% of the predictions correct.

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/UnderSampling_balanced%20Accuracy%20score.png?raw=true)


[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/UnderSampling_classification%20report.png)

**The precision** 
This measure is not of use in our analysis due to biases as explained above.

**The recall (sensitivity)** in predicting "bad credit is 59% where the "good credit" prediction is 43%. Overall, the model predicted 43% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/UnderSampling_classification%20report.png?raw=true)

#
### 4. Combination (Over and Under) Sampling
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/CombinationSampling_balanced%20Accuracy%20score.png)

Combination sampling suggests 64.8% accuracy score. This means the model generated 64.8% of the predictions correct.


![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/CombinationSampling_balanced%20Accuracy%20score.png?raw=true)


[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/CombinationSampling_classification%20report.png)

**The precision** 
This measure is not of use in our analysis due to biases as explained above.

**The recall (sensitivity)** in predicting "bad credit is 71% where the "good credit" prediction is 59%. Overall, the model predicted 59% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/CombinationSampling_classification%20report.png?raw=true)

#
### Ensemble Learners
#### 5. Balanced Random Forest Classifier
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/BalancedRandomForestClassifier_balanced%20Accuracy%20score.png)

The model suggests 72.3% accuracy score. This means the model generated 72.3% of the predictions correct.

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/BalancedRandomForestClassifier_balanced%20Accuracy%20score.png?raw=true)


[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/BalancedRandomForestClassifier_classification%20report.png)

**The precision** 
This measure is not of use in our analysis due to biases as explained above.

**The recall (sensitivity)** in predicting "bad credit is 57% where the "good credit" prediction is 88%. Overall, the model predicted 88% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/BalancedRandomForestClassifier_classification%20report.png?raw=true)

#### 6. Easy Ensemble AdaBoost Classifier
[**Balanced Accuracy Score**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/EasyEnsembleAdaBoostClassifier_balanced%20Accuracy%20score.png)

The model suggests 72.3% accuracy score. This means the model generated 72.3% of the predictions correct.

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/EasyEnsembleAdaBoostClassifier_balanced%20Accuracy%20score.png?raw=true)


[**Classification Report**](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/EasyEnsembleAdaBoostClassifier_classification%20report.png)

**The precision** 
This measure is not of use in our analysis due to biases as explained above.

**The recall (sensitivity)** in predicting "bad credit is 57% where the "good credit" prediction is 88%. Overall, the model predicted 88% correctly. 

![](https://github.com/neerajain9/Credit_Risk_Analysis/blob/Data-Science/Resources/EasyEnsembleAdaBoostClassifier_classification%20report.png?raw=true)


## Summary
1. Random Oversampling predicted with 61.9% accuracy, 58% recall, and 73% F1 score. This isn’t terrible if not too good.
1. SMOTE Oversampling outperformed Random Oversampling with 63.9% accuracy, 65% recall, and 78% F1 score. This are **reasonable predictions**.
1. Under sampling predicted with 50.6% accuracy, 43% recall, and 59% F1 score. This model **underperformed**.
1. Combination sampling predicted with 64.9% accuracy, 59% recall, and 74% F1 score. This model made **reasonable predictions**.
1. **Balanced Random Forest Classifier**, and **Easy Ensemble AdaBoost Classifier** models  predicted with 72.3% accuracy, 88% recall, and 93% F1 score. **These model outperformed rest of the other model’s predictions.**

#
### Recommendations
We recommend using either of the Balanced Random Forest Classifier or Easy Ensemble AdaBoost Classifier models based on above analysis.