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

* RandomOverSampler:

  * Balanced Accuracy Score: 0.62
  * Precision: 0.99
  * Recall Score: 0.68

<img src=“images/random_oversampling.png” alt="Alt text" title="Optional title" width="450" height="250"/>

 
* SMOTE algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: 0.99
  * Recall Score: 0.66

<img src=“images/smote.png” alt="Alt text" title="Optional title" width="450" height="250"/>
 
  
* ClusterCentroids algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: 0.99
  * Recall Score: 0.66

<img src=“images/clustered.png” alt="Alt text" title="Optional title" width="450" height="250"/>
 

* SMOTEENN algorithm:

  * Balanced Accuracy Score: 0.63
  * Precision: 0.99
  * Recall Score: 0.66

<img src=“images/smoteenn.png” alt="Alt text" title="Optional title" width="450" height="250"/>
 

* BalancedRandomForestClassifier:

  * Balanced Accuracy Score: 0.67
  * Precision: 0.99
  * Recall Score: 0.91

<img src=“images/brfc.png” alt="Alt text" title="Optional title" width="450" height="250"/>
 

* EasyEnsembleClassifier:

  * Balanced Accuracy Score: 0.91
  * Precision: 0.99
  * Recall Score: 0.94

<img src=“images/eeac.png” alt="Alt text" title="Optional title" width="450" height="250"/>
 


# Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
