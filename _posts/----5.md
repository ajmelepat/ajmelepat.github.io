---
layout: post
author: Harika kanthi
title: Logestic Regression
date: 2020-10-10T05:25:16.594Z
thumbnail: /assets/img/posts/diagram-2008478_640.png
category: Machine Learning
summary: Basics of Logestic Regression
---


**Confusion matrix:**

A most intuitive metric for finding the correctness and the accuracy of the model.

It can be used in classification problems where the output can be of two or more types of classes.

It is matrix of predicted values against the actual values.

True positives: The classes which are positive and are detected to be positive

True negatives: The classes which are negative and are detected to be negative

False positives: The classes which are actually negative but have been falsely detected as positive

False negatives: The classes which are actually positive but have been falsely detected as negative





**Evaluation metrics:**



***Accuracy:*** The total number of current predictions are made by the model.

Accuracy = TP+TN / TP+TN+FP+FN

It is not a very good feature in case of class imbalance because the model will be able to predict more of the majority class.



***Precision:*** The proportion of correctly predicted positive classes of the predicted positive class.

**Precision = TP / TP+FP**

***Recall or sensitivity:*** or True positive rate The proportion of correctly predicted positive classes of the actual positive class.

**Recall = TP / TP+FN**

***Specificity:*** The proportion of correctly predicted negative classes of the actual negative class.

**Specificity = TN / TN+FP**

***F1 score:*** The combination of both precision and recall. It is the harmonic mean.

**F1 score = (1/ precision + 1/recall)/2 = 2\*precision\*recall / precision+recall**

False positive rate: The proportion of falsely predicted negative classes of the actual negative class.

**FPR = FP/TN+FP**



***Roc auc:***

Auc = area under the curve = area under the receiver operating characteristic curve

It lies between 0 or 1.

The model where predictions are 100% wrong, auc is 0 while when all are predicted correctly we get an auc of 1.

Roc = receiver operating characteristic

It is a curve plotted with total positive rate against False positive rate