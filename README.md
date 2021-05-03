# Credit Risk Analysis
## Overview
The purpose of this analysis is to compare multiple forms of machine learning prediction techniques to determine the most effective method of predicting loan approval (Y/N) based on provided data.

## Results

* **Naive Random Oversampler*
    * Balanced Accuracy Score: 64.62% 
    * Precision: 99%
    * Recall: 66%

* **SMOTE Oversampling*
    * Balanced Accuracy Score: 61.20%
    * Precision: 99%
    * Recall: 63%

* **Cluster Centroids Undersampling*
    * Balanced Accuracy Score: 51.60% 
    * Precision: 99%
    * Recall: 44%

* **Combination (SMOTEENN) Sampling*
    * Balanced Accuracy Score: 63.64%
    * Precision: 99%
    * Recall: 58%

* **Balanced Random Forest Classifier*
    * Balanced Accuracy Score: 78.78%
    * Precision: 99%
    * Recall: 91%

* **Easy Ensemble AdaBoost Classifier*
    * Balanced Accuracy Score: 92.54% 
    * Precision: 99%
    * Recall: 94%

## Summary
In conclusion, the Ensemble Classifier and the Random Forest Classifier models greatly outperformed the other models in prediciton accuracy. 

For this problem space (loan risk assessment) we would want a system that erred on the side of caution, so that we would be more likely to NOT give a loan to someone who might erroneously classified as qualified. That means we might weigh the sensitivity ("recall") score higher than the precision value in determining which model to use. 

**Recommendation:** The Easy Ensemble AdaBoost Classifier is the clear winner out of these models, with a high accuracy, precision, and sensitivity value. The previous note about weighing recall more heavily in our considerations does not actually need to be factored into this decision, as the model is superior in all noted metrics.