---
layout: post
author: Harika kanthi
title: Linear Regression
date: 2020-10-10T04:50:08.974Z
thumbnail: /assets/img/posts/graph-3186077_640.png
category: Data Science
summary: Basic understanding on Linear Regression
---
<!--StartFragment-->

**Supervised learning?**

The task of learning where we have a prediction to be made given a set of predictor features.

It can be of two types:

**Regression and classification**

Regression is where we try to learn the data related to a continuous dependent feature.

While classification

e.g. linear regression



**Unsupervised learning?**

Unsupervised learning is a task of learning underlying patterns in the data given a set of features.

e.g. clustering



**Semi-supervised learning?**

A task of learning the data which has a large amount of data of which only few are labelled.

e.g. labelling audio files.

Usually whenever the tasks are human intensive.



**Occums razor rule**

It states that simple solutions are more likely to be correct than complex ones.



**Parametric Non-parametric models?**

**Parametric:**

A model that learns a set of parameters of a fixed size is called a parametric model.

It has an underlying function to it.

e.g. Linear regression is a parametric model because it learns the coefficients and the intercepts of the best fit line

* Linear regression
* Logistic regression
* Naïve Bayes



**Advantages:**

* Simple
* Speed
* Not much data is required



**Limitations:**

* Constrained to the specific form
* Limited complexity
* Poor fit



**Non-parametric:**

These algorithms do not have any strong assumptions about the data. They work good when we have large data and no prior knowledge.

e.g. Knn algorithm learns the data and predicts the data based on the nearest neighbours

* K nearest neighbors
* Decision trees
* Support vector machines



**Advantages:**

* Flexibility
* No assumptions
* Performance
* No scaling is necessary



**Limitations:**

* More data
* Slower
* Overfitting



**Strong and weak learners?**

Weak learners is the classifier which performs poorly.

For example, when the data is does not have a linear relationship associated with the dependent feature, in such case linear regression is a weak learner.

But in case of good linear relationship between the features and the dependent feature, linear regression is a strong learner.





**Overfitting and underfitting?**

Overfitting refers to a model that learns every detail in the data including the noises. That is when the model learns the details of the training data to an extent where it negatively impacts the performance of the model on the new data.

It is more likely with non-parametric and non-linear models because they have more flexibility while learning a target function.

To deal with over fitting we can use:

* Cross validation
* More data
* Feature removal
* Early stopping
* Regularization
* Ensemble



Underfitting happens when a model is unable to capture the true relationship of the features.

It is not a suitable model as it will have poor performances on both training data and test data.

To deal with underfitting:

* Add new features in the data
* Increase complexity in the model
* Increase training time until cost function is minimised.









**Noise, bias , variance?**

***Noise*** is the distortion or the redundancy in the data. Anything that is not useful and that is limiting the use of the learning of the model is said to be noise. By noise we mean the data points that don’t really represent the true properties of your data.



***Bias*** error is the error made by the model while learning the data. Bias simplifies the assumptions made by model on the data. Typically simpler models have higher bias.The error made by the model because it is prejudiced to faulty assumptions.

High bias : more assumptions about the target function. e.g. linear regression, logistic regression

Low bias: less assumptions about the target function. e.g. Decision trees, KNN, SVM

To deal with it:

* Complex models
* Boosting techniques



***Variance*** is the error made by the model while predicting unseen data.

More complex model tends to have higher variance. Variance deals with the consistency in the data.

Low variance: small changes to the estimate of target function with changes in data. e.g. Linear regression, logistic regression

High variance: large changes to the estimate of target function with changes in data. e.g. KNN, Decision trees etc.

To deal with it:

* Simpler models
* Bagging techniques







**Bias Variance trade-off?**

The goal of any algorithm is to achieve low bias and low variance for a good performance. Linear algorithms often have large bias and low variance. Non-linear algorithms often have a low bias and high variance. The choice we need to make in order of trade bias for variance is called as bias variance trade off







**Regression?**

Regression is a technique that involves a dependent feature Y and independent features X where we try to find relationship between the dependent and the independent features.

Typically In regression the dependent feature that is the feature we are trying to predict is continuous in nature.







**Dependent and Independent features?**

***Dependent features*** are explained the name itself. These features depend on other features which we call the independent features.

They are also called the prediction feature or target feature.

e.g. Income is a dependent feature while age, experience etc will be its independent features.



***Independent features*** as the name suggests are independent and are used to measure a dependent feature.

They are also called as predictor features.

e.g. Age is an independent feature in income prediction







**Linear Regression?**

Linear regression is a method used to model the relationship between dependent continuous feature and its respective independent features. It was developed in statistics to understand relationship between the dependent and independent features. It was borrowed by machine learning. Hence it is both statistical and a machine learning algorithm as well.





**Assumptions of linear regression?**

* ***Linearity:*** A linear relationship must exist between the dependent and independent features. Can be found using scatterplots and correlation.
* ***Independence of errors(No Autocorrelation) :*** No correlation between the values of same variables across different observations in the data. Durbin Watson test is a method to find the autocorrelation where the values range between 0 and 4. When the values are closer to 2, it implies no autocorrelation. If values are greater than 2, it implies a positive autocorrelation. IF values are less than 2, it implies negative autocorrelation.
* ***Normality of errors:*** The errors we get after fitting a regression model should follow a normal distribution. A distribution plot of the errors can help us see the normality.
* ***Homoscedasticity (No Heteroscedasticity):*** The variance around the regression line should be the same for all the values.
* ***No Multicollinearity:*** The independent variables should not be dependent on each other as they will add noise to the data.







**Loss Function ?**

The loss function or the cost function is a measure of how good a prediction model is in terms of explaining the prediction. It is of two kinds:

Classification and regression

* In regression, the loss function is mean squared error.
* In classification, the loss function is log loss.





**Ordinary Least Squares method?**

This is a type of linear regression where we try to find the best fit line for the features where the mean sum of squares of errors is the least.





**Simple linear regression?**

This kind of regression has only one independent and one dependent features.

e.g. Trying to find income based on experience.



**Multiple linear regression?**

This kind of regression has more than one independent and one dependent features.

e.g. trying to predict income with education , age, experience etc.





**Regression best fit line equations?**



f(y) = b0+b1x1+b2x2+…..+ bnxn

N = number of features

B0 = intercept

b1,b2,…. = coefficients

y= prediction or target feature

x= independent features.





**Gradient descent:**

A method of linear regression which is an optimization technique.

When we calculate the loss function foe every conceivable value of weights over the entire dataset, it will form a parabola.

Using this the gradient descent tries to find the least error.

It starts at a random point and calculates the cost function. It then uses differentiation on the slope of the curve and tries to find the least value in the curve.

When the least value is found the iteration stops.

This method is computationally expensive.





**Stochastic Gradient Descent:**

It is a kind of gradient descent method which is an optimisation technique.

In this method, similar to the gradient descent it also tries to find the least error i.e. the least cost function.

It is much faster than Gradient descent as the computation is faster.



Advantages:

* Faster in computation

Disadvantages:

* Might skip the actual global minima
* Will stop immediately when the iterations are finished.





**Local minima and global minima:**

Global minima is the value at which the loss function is minimum globally across the entire data. There can be only one be







Evaluation metrics in regression:

* Mean Absolute error: The simplest evaluation metric to measure the error between the actual and predicted values. It is the average absolute deviation in the errors.

MAE = 1/n sigma(abs(yactual -ypred))



* Mean square error: The evaluation metric to measure the average squared difference between actual and predicted values.

MSE = 1/n sigma(yactual - ypred)\*\*2

* Mean Absolute percentage error: The evaluation metric which is equal to the percent equivalent of the mean absolute error. Every error is scaled against the actual value.

MAPE = 100%/n sigma(abs(yactual - ypred)/yactual)

* Mean percentage error: The evaluation metric which measures the percentage of error caused. It calculates the error which is scaled.

MPE = 100%/n sigma ((yactual - y pred)/yactual)

* Symmetric mean absolute percentage error: The evaluation metric which is an absolute difference between actual and predicted values.

SMAPE = 100%/n sigma abs(actual-pred) / (actual+pred)/2





**Generalisation:**

It refers to the ability of the model to adapt itself to new unseen data, drawn from the same distribution as the one used to create the model.

After being trained on a training set, a model needs to predict the new unseen data. When the model overfits or underfits we need to generalise the model in order to find the model with the least bias and variance errors.

Such a model is called a generalised model.





**Regularisation:**

A method of generalisation which helps reduce overfitting in case of linear regression methods.

This technique shrinks the coefficient estimates towards zero in order to avoid the risk of overfitting.

Regularization, significantly reduces the variance of the model, without substantial increase in its bias.

The increase in λ is beneficial as it is only reducing the variance(hence avoiding overfitting), without loosing any important properties in the data

It is of two types:

1. Ridge regression
2. Lasso regression



**Ridge regression:**

This is a type of regularisation technique which allows a penalisation of the coefficients by minimising the cost function.

It adds a shrinkage quantity. The coefficient estimates will approach zero but will never become zero.







**Lasso regression:**

This is a type of regularisation technique which allows a penalisation of the coefficients by minimising the cost function.

It adds a shrinkage quantity. The coefficient estimates will approach zero. This also has an ability to make the coefficients zero.

It is a method of feature selection or a dimensionality reduction technique.