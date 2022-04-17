# Credit_Risk_Analysis

The purpose of the credit risk analysis is to develop several different machine learning models in order to assess credit risk for borrowers. The purpose of employing several models rather than just one or two because each algoritm as irs own advantages and disadvantages. Therefore, in order to assess the algorithm and model that best fits our dataset, several models were employed and evaluated. By doing so, the model can be used in the future for similar scenarios involving credit risk amongst financial institutions.

## Tools

Terminal (Mac), Jupyter Notebook

#### Dataset: 
LoanStats_2019Q1.csv (from LendingClub)
#### Libraries:
sckit-learn, imbalanced-learn, pandas, numpy

# Results

Six machine learning models were evaluated for this analysis: RandomOverSampler, SMOTE algorithm, ClusterCentroids algorithm, SMOTEENN algorithm, BalancedRandomForestClassifier, and EasyEnsemble Classifier. Images of the outputs for each model are used to supplement this analysis. Outputs for each model were calculated from the imbalanced classification report. This method was iported from imblearnmetrics.

* ## RandomOverSampler:

  * Balanced Accuracy Score: 0.62
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.68

![Pic 1](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/random_oversampling.png)     


* ## SMOTE algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.66
  
 ![Pic 2](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/smote.png)
 
  
* ## ClusterCentroids algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.66

 ![Pic 3](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/clustered.png)


* ## SMOTEENN algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.66


 ![Pic 4](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/smoteenn.png)


* ## BalancedRandomForestClassifier:

  * Balanced Accuracy Score: 0.67
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.04 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.91

 ![Pic 5](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/brfc.png)
 

* ## EasyEnsembleClassifier:

  * Balanced Accuracy Score: 0.91
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.07 and low-risk loans had a high   precision 1.00.
  * Recall Score: 0.94
 
  ![Pic 6](https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/eeac.png)


# Summary

The three metrics used to described each machine learning model are balanced accuracy score, precision, and recall score. Balanced accuracy score is defined as the average of recall obtained on each class. The best balanced accuracy value is 1 and the worst value is 0 when adjusted=False. Of all the six machine learning models produced, EasyEnsembleClassifier had the highest balanced accuracy value of 0.91. The lowest of that score was demonstrated in the RandomOverSampler model. Next, the precision of each model is the ratio of true positives to the sum of true and false positives in numerical format. The same average average precision score is demonstrated in all models, however, the most important aspect of the precision is that which reflects high-risk and low-risk loans. All the low-risk loans had a high precision of 1.00 and the relatively best high-risk precision is exhibited in the EasyEnsembleClassifier model with a value of 0.07. This value is only slightly higher than the other models and is considered statistically low. Lastly, recall score measures the ability of a classifier to find all positive instances. In other words it is the fraction of positives that were correctly identified. A good classifier should have a score of 1, and a poor classifier would have a score closer to 0. EasyEnsembleClassifier shines through again with a high recall 




Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
