# Credit_Risk_Analysis

Using Supervised Machine Learning to analyze credit risk data.

## Overview of the analysis:

The purpose of the analysis is to determine the most effective algorithm, using Supervised Machine Learning, to assist LendingClub in their future lending assessments. The algorithms used in the analysis are:

- RandomOverSamlper
- SMOTE
- ClusterCentroids
- SMOTEENN
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

(Used Jupyter Notebook to perform the analysis)

## Results:

The balanced accuracy scores and the precision and recall scores of all six machine learning models. Using screenshots of the outputs to support the results.

* Each algorithm in order and images of the accuracy scores and classification reports.

### CLusterCentroids

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/ClusterCentroids_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/ClusterCentroids_classification.png">

</p><br/>

- Accuracy Score of 54.4%. This is too low.
- Precision Score is low for high_risk loans and high for low_risk loans.
- Recall Score's are also on the low end indicating a greater chance of false negatives.

### RandomOverSampler

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/RandomOverSampler_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/RandomOverSampler_classification.png">

</p><br/>

- Accuracy Score of 64.6%. Better but still not great.
- Precision Score's are still very low for high_risk and high for low_risk.
- The Recall is slightly better than previously but still too low.


### SMOTEENN

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/SOMTEENN_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/SOMTEENN_classification.png">

</p><br/>

- Accuracy Score of 64%. No better than the RandomOverSampler.
- Again the Precision Score is low for high_risk and high for low_risk.
- The recall scores for both high and low risk have improved slightly, but still not a great candidate.

### SMOTE

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/SMOTE_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/SMOTE_classification.png">

</p><br/>

- Accuracy Score of 65.8%, slight improvement.
- The Precision Score is once again the same for high and low risk.
- The recall score for low_risk has improved but now the high_risk has dropped.

### BalancedRandomForestClassifier

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/BalancedRandomForestClassifier_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/BalancedRandomForestClassifier_classification.png">

</p><br/>

- Accuracy Score of 78.8%. Much better than any previous score.
- The Precision Score has improved for high_risk and stayed the same for low_risk.
- The recall scores improved a lot, but the high_risk could be better.

### EasyEnsembleClassifier

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/EasyEnsembleClassifier_accuracy.png">

<p align="center">
<img src="https://github.com/mehill37/Credit_Risk_Analysis/blob/23f76a5549ce63e64ae70422c1ac9b0e3708047f/images/EasyEnsembleClassifier_classification.png">

</p><br/>

- Accuracy Score of 93.1%. The best option so far.
- Precision Score is the best out of all the options as well.
- The recall scores have also improved immensely. High and low risk are both high scores lowering the chances of false negatives.

## Summary: 

It's clear from the results found that the best Machine Learning Model is EasyEnsembleClassifier for LendingClub to use. The scale for these measures is 0 to 1. The closer to 1 the more successful the measure. This needs reassessed routinely when new techniques are developed to make sure its still the best Model. 
