# Credit_Risk_Analysis

The purpose of the credit risk analysis is to develop several different machine learning models in order to determine which model best assesses credit risk for borrowers. The dataset used in the analysis, LoanStats_2019Q1.csv, is provided by LendingClub. The purpose of employing several models rather than just one or two is that it allows financial institions to compare and determine the best model. By doing so, this may reduce potential bias and reduce their own risk of lending to high-risk borrowers. To assess which model best fits our dataset, six machine learning models were employed, evaluated, and compared with each other. 

## Tools

Terminal (Mac), Jupyter Notebook

#### Dataset: 
LoanStats_2019Q1.csv (from LendingClub)
#### Libraries:
scikit-learn, imbalanced-learn, pandas, numpy

# Results

Six machine learning models were evaluated for this analysis: RandomOverSampler, SMOTE algorithm, ClusterCentroids algorithm, SMOTEENN algorithm, BalancedRandomForestClassifier, and EasyEnsemble Classifier. Images of the outputs for each model are used to supplement this analysis. Outputs for each model were calculated from the imbalanced classification report. This method was imported from imblearnmetrics.

* ## RandomOverSampler:

  * Balanced Accuracy Score: 0.62
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.68

<img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/random_oversampling.png" width="600" height="220" />        

* ## SMOTE algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.66
  
<img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/smote.png" width="650" height="250" />     
 
  
* ## ClusterCentroids algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.66

<img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/clustered.png" width="650" height="250" />   


* ## SMOTEENN algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.01 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.66


<img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/smoteenn.png" width="650" height="250" />     


* ## BalancedRandomForestClassifier:

  * Balanced Accuracy Score: 0.67
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.04 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.91

<img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/brfc.png" width="650" height="250" />     
 

* ## EasyEnsembleClassifier:

  * Balanced Accuracy Score: 0.91
  * Precision: The average precision score is 0.99. Separately, the high-risk loans had a low precision of 0.07 and low-risk loans had a high   precision of 1.00.
  * Recall Score: 0.94
 
 <img src="https://github.com/katmarcin/Credit_Risk_Analysis/blob/049173235bb3cdca6fed8744575ed8b4142fa518/images/eeac.png" width="650" height="250" />     


# Summary

The three metrics used to described each machine learning model are balanced accuracy score, precision, and recall score. Balanced accuracy score is defined as the average of recall obtained on each class. The best balanced accuracy value is 1 and the worst value is 0 when adjusted=False. Of all the six machine learning models produced, EasyEnsembleClassifier had the highest balanced accuracy value of 0.91. The lowest of that score was demonstrated in the RandomOverSampler model. Next, precision of each model is calculated by the ratio of true positives to the sum of true and false positives in numerical format. The same average average precision score is demonstrated in all models, however, the most important aspect of the precision is that which reflects high-risk and low-risk loans. All the low-risk loans had a high precision of 1.00 and the relatively best high-risk precision is exhibited in the EasyEnsembleClassifier model with a value of 0.07. This value is only slightly higher than the other models. Lastly, recall score measures the ability of a classifier to find all positive instances. In other words, it is the fraction of positives that were correctly identified. A good classifier should have a score of 1, and a poor classifier would have a score closer to 0. EasyEnsembleClassifier shines through again with a high recall score of 0.94. The lowest recall score, 0.66, is exhibited amongst the SMOTE, ClusterCentroids, and SMOTEENN algorithm models.

For further credit card risk analysis, it would be best to proceed with the EasyEnsembleClassifier model, which exhibited relatively high scores amongst all major metrics and therefore it performed the best. It is important to choose this model as it implements an algorithm that reduces bias and is also both precise and accurate in calculating credit risk. Financial institutions must have proper credit risk management and modeling to prevent false negatives, aka high-risk loans that are misinterpreted asprospective low-risk loans. 


