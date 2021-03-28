# Module 12 Report
## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis is to weed out risky loans classified by machine learning methods of classification. The method used is Logistic Regression and comparatively an OverSampled re-run of the data through the imlearn library. The analysis determines risky loans through supervised learning of a credit risk data set of good and bad loans.

Variables needed to predict are '1' for bad credit and '0' for good credit.

Steps in the process:
* reading in data
* splitting data into training and testing for the model
* creating the model
* scaling the data for the model
* fitting and traning the model based on known data
* making predictions based on the model with known data
* comparing the predictions to the trained model that was based on the known data

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.

PRE: precision - positive prediction value (values of 1)
REC: recall - sensitivty to the data provided
SPE: specificity - True Negative Rate (values of 0)
f1: f1 Score - Harmonic mean of precision and sensitivity/recall
geo: geometric mean
iba: imbalance

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
![image](https://user-images.githubusercontent.com/75395061/112766862-8b67d100-8fc8-11eb-8cc0-0330322851f3.png)

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
![image](https://user-images.githubusercontent.com/75395061/112766883-a0dcfb00-8fc8-11eb-8319-55e4ce11e594.png)

## Summary

The most important target for prediction is the bad credit cases which are denoted with  a '1'.

Although both models seem to output relatively the same accuracy, but through the Oversampling of the data, there are slightly less false negatives and false positives of the predicted cases. The most important data is the false negatives in this case, as we do not want to approve of a loan that is bad but is predicted negative denoted by a '0'. Both models seem to have very small differences in the predicted false negatives so either model works or we should find another model/metric to judge the data on.
