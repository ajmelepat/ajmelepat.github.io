---
layout: post
author: Harika kanthi
title: Bagging And Boosting
date: 2020-10-10T06:00:47.837Z
thumbnail: /assets/img/posts/money-4029562_640.png
category: Machine Learning
summary: Bagging and Boosting
---
<!--StartFragment-->

**Ensemble:**

The machine learning technique which combines several base models in order to produce one optimal predictive model.

It brings weak learners together to create a strong learner.

It is of two types:

Bagging

Boosting





**Bootstrap:**

A resampling technique which is used to sample with replacement





**Bagging:**

Also called Bootstrap Aggregation. It build models parallelly reducing variance. An ensemble technique which combines predictions from multiple models and makes a more accurate prediction. It is a method that is used to reduce the variance in high variance algorithms like decision trees



**Steps:**

* Selects k samples using bootstrap
* Builds classifiers or regressors on each sample
* Combines the classifiers
* Tests the data and gives predictions

In case of classification voting method is used while for regression mean is used





**Random Forest:**

A special kind of bagging technique where we can bootstrap the features as well. It bootstraps both observations and features. It is a collection of decision trees.

The features are bootstrapped where in :

For classifications default = m = sqrt(p)

For regression default = m = p/3



**Steps:**

1. Create bootstrapped data
2. Create decision trees
3. Go to step 1 and repeat until all iterations are completed.
4. Predict the new data
5. Evaluate the model



**Out of bag(OOB)?**

OOB is the out of bag data that is the data left after bootstrapping. OOB score is the score of correctly predicted observations of the out of bag sample. The difference from validation set is that it is predicted on unused observations in the data. Whereas validation is already set aside before we train the model.







**Up sampling and down sampling?**

The method of sampling so that we can deal with the class imbalance in the data.

Up sampling is when we increase the observations in the minority class while down sampling is reducing the majority class observations.





**SMOTE - Synthetic minority oversampling technique?**

A method of oversampling the minority class

It creates new minority instances between real minority observations.

Step1: sets the minority class, and the k nearest neighbours of the minority class by calculating Euclidean distance

Step 2: the sampling rate is set according to the imbalanced proportion.

Step 3: generates the sample





**Near miss?**

A method of under sampling the minority class

Step1: calculates distances between all instances of majority class and the minority class.

Step2: n instances of majority class have the smallest distances to the minority class

Step3: if there are k instances in minority class, the nearest method will result in k*n instances od majority class.

Ways to select the instances:

K closest

K farthest

For each minority instance m nearest are selected





<!--EndFragment-->