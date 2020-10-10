---
layout: post
author: Harika Kanthi
title: Algorithms
date: 2020-10-10T05:37:08.237Z
thumbnail: /assets/img/posts/tree-684764_640.jpg
category: Machine Learning
summary: Understanding on algorithm
---
# KNN (K Nearest Neighbors)

It is a supervised learning algorithm which can be used for both classification and regression.

It is mainly used for classification predictions.

It can be defined as :

***Lazy learner:***

It is a lazy learning algorithm because it does not have a training phase

***Non parametric:***

It is non parametric as it does not have any underlying assumptions.

Imp: scaling is important for a KNN algorithm

***Working:***

The knn algorithm helps predict the unseen data based on the neighbours selected.

**Step1:** loading the dataset

**Step2:** choose the k nearest neighbours. It can be any integer.

When the k value is 1, it overfits as it is applying the value of the most nearest neighbour to the new point.

But if k is equal to n, it underfits as it is applying the average value of the dependent feature to the new point.

K value can be anyway around less than 10% of the observations.

**Step3:** for each point in the test data:

* Distance between the test point and the training data points with the help of Euclidean, Manhattan or hamming distance. The most common used method to calculate distance id Euclidean.
* Based on the distance value, sort them in ascending order
* Choose top k rows from the sorted array
* Assign the class based on majority or the average in case of regression

**Pros:**

* Very simple to interpret and understand
* No assumptions underlying the data
* Versatile cause it can be used for both classification and regression
* Relatively high accuracy

**Cons:**

* Computationally bit expensive algorithm
* High memory storage
* Prediction is slow in case of large number of observations
* Very sensitive to scale of data as well as irrelevant features.

***Applications:***

Banking approval: to predict weather an individual is fit for loan approval?

Does the individual have same characteristics as defaulters?

Knn can be used for

* Speech recognition
* Handwriting detection
* Image recognition
* Video recognition

![](/assets/img/posts/knn_similarity.png)

![](/assets/img/posts/knn_hamming.png)

**Hyper parameters in KNN?**

* K neighbors
* Distance

<!--EndFragment-->

<!--StartFragment-->

## Naive Bayes

The naive bayes classifier is based on Bayes' theorem between independent and the dependent features. This is easy to build, because it has no complicated parameter estimation which makes it useful for large datasets. Despite being simple, it works well and is widely used because it outperforms more sophisticated models.



**Bayes theorem:**

Bayes theorem is calculates the posterior probability, p(A|B) from P(A),P(B) and P(B|A).

![](/assets/img/posts/bayes_rule.png)



P(c|x) is the posterior probability of class (target) given predictor (attribute).

P(c) is the prior probability of class.

P(x|c) is the likelihood which is the probability of predictor given class.

P(x) is the prior probability of predictor.





Naïve bayes classifier assumes that the effect of the value of the predictor on a given class is independent of the values of the other predictors. This assumption is called conditional independence.

It includes all independent features using bayes theorem.





**Assumptions:**

* Conditional independence of features
* Normality of numerical distributions





**Zero frequency problem?**

When every attribute does not have a combination with every class it is a zero frequency problem.

To deal with it, 1 is added to such attribute-class combination.





**Gaussian naive bayes:**

Simplest naïve bayes classifier having assumption that the data is drawn from a simple gaussian distribution.



**Multinomial naive bayes:**

When the features are assumed to be drawn from a multinomial distribution. It is very appropriate for discrete counts.



**Bernoulli naive bayes:**

When the features are assumed to be binary, such as text classification, it is called Bernoulli naïve bayes.



**Pros:**

* Faster and easy to implement
* Converges faster than discriminative models like logistic regression
* Requires less training data
* Can handle both continuous and discrete data
* Can be used for binary and multi class classification

**Cons:**

* Strong conditional independence which is almost impossible
* If a categorical feature has a category not observed in training data, it will assign zero probability and cannot make prediction



**Applications:**

* Real time predictions
* Multi class predictions
* Text classification
* Recommendation systems







**Why Naive Bayes is not a good regressor and Why Naive Bayes Model is called Naïve?**

It is called naive because it assumes conditional independence that is that the features are independent of each other.

It is a naive because it is almost never true.

<!--EndFragment-->

### Decision Tree

<!--StartFragment-->

Decision trees are the models that learn the data by building tree like structure.

It divides the data into smaller subsets and develops the tree.

The final tree has decision nodes and leaf nodes.

It can be used effectively in both regression and classification.

It can handle both numerical and categorical data.



**Pros:**

* Easy to interpret and explain to nontechnical users
* Require relatively less effort for data preparation
* Implicitly perform feature selection

**Cons:**

* Without proper pruning, they will tend to overfit the data making them poor predictors
* Attributes with many unique values
* Working with missing values
* Imbalanced classes



**Objective:**

Reduce impurity in classification models

Reduce standard deviation in case of regression models.

Sd = sqrt ( sigma ( x-xbar)\*\*2/n)

Cv = coefficient of variation = s/x *100%



**Gini Index:**

The cost function used to evaluate the splits in the algorithm.

Higher the Gini index, higher the homogeneity.

It is a measure of impurity in the node.

A node with multiple classes is impure while the one with homogenous classes is pure.

Gini = 1- sigma p(c )\*\*2

P(c ) is the probability of class i in the node.



**Entropy:**

A measure of impurity in the node.

A branch with entropy zero is a leaf node

It cannot be split further

Entropy = sigma ( -p* log p )



**Information gain:**

It is a measure of how much information we are able to gain by doing the split

IG (T,X) = entropy(T) - entropy(T,X) "classification"

S(T,X) = sigma\[ P(i) S(i) ] for I in X "regression"







**Assumptions:**

* Training set is the root node
* Prefers values to be categorical







**Why dt has high bias?**

Decision trees tend to be biased towards the domination class.

That is information gain for a decision tree with categorical features gives a biased response for features with greater number of categories.





**Why dt has high variance?**

Decision trees build very large trees until all homogeneous nodes are found.

In this process it learns the entire training data which works very good on a training data making it overfit.

As a result it will not work better on the test data producing high variance.





**Why dt is base estimator for bagging and bosting?**

The ensemble methods are one of the best methods which benefit on decision trees while reducing its ability to overfit.

The bagging and boosting methods create decision stumps randomly.

Decision stumps are weak learners or base learners.

They are used in ensemble methods as base estimators.







**What is explainability in data science?**

The extent to which the features are able to explain the variability in the dependent feature is called as explainability.



**What is variability in data science?**

The spread of the data is called as variability.







Terminologies:



**Root node:** the entire sample or population with which we start the decision tree structure.

**Splitting:** The processing of dividing a node into two or mode sub nodes

**Decision node:** When a sub node gets further divided into further sub nodes, it is called a decision node

**Leaf node:** Also called the terminal node is the last node or the nodes which do not split further.

**Pruning:** the process of removing the sub nodes is called pruning. It can be of two types pre and post.

**Pre pruning:** The process of early stopping of the splitting process is called pre pruning.

**Post pruning:** The process of stopping the tree after building the entire tree is called post pruning.

**Parent Node:** A node which is being divided

**Child node:** The sub nodes of a parent node

**Decision stump:** the decision tree with only one level is known as decision stump.





**Applications:**

* Business management
* Fraud detection
* Healthcare management





**Steps:**

1. Loading the data into the algorithm creating the root node
2. The feature which best explains that is with the lowest impurity is used to split the data into sub nodes.
3. The process continues until pure homogenous nodes or leaves are created.





**Feature importance:**

The decrease in the node impurity weighted by probability of reaching that node is the feature importances.

The node probability can be calculated by dividing the number of samples in the node by total number of samples

Higher the value important the feature.





**Hyper parameters?**

* Min samples in a leaf
* Min splits
* Criterion
* Maximum depth





<!--EndFragment-->