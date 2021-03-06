---
layout: post
author: Ajay M
title: Basics of Statistics for machine learning
date: 2020-07-23T11:48:30.197Z
thumbnail: /assets/img/posts/code.jpg
category: Statistics
summary: Basics of Statistics
---
STATISTICS

Statistics plays a very crucial part in understanding the data. It was developed in the 17th to 19th centuries. Challenges in the areas of data analysis and organisation have been given a scope due to the statistical influence in data science. Vast amounts of data is being generated and it is the job of the researcher to make sense of the data. It helps us understand the main question “What does the data tell?”

Statistics can be divided into three categories:
1.	Descriptive statistics: The statistical measures that help describe the data. Often used to present the results.
2.	Inferential Statistics: The statistics that uses the descriptive measures to infer the data and patterns related.
3.	Predictive Statistics: The statists that help predict the event based on the inferences from the inferential and the descriptive statistics.


Main terminologies in statistics:
1.	Population: The complete set of observations that belong in the study based on the criteria chosen.
e.g. People who smoke in Hyderabad of age 20
It includes all people with age 20 and from Hyderabad and they smoke.

2.	Sample: The part of a population which has been extracted or selected such that it represents the population that is it follows the same criteria as the population. It is usually selected through different means as selecting the entire population is computationally impossible.
e.g. From the same example from population where criteria are people of age 20 from Hyderabad who smoke.
In this we select a part of population of about let’s say 20000 people who are of age 20, from Hyderabad and smoke.

3.	Parameter:  The characteristics of a population are called parameter.
e.g. mean of population is denoted as “μ “ 
     standard deviation is denoted as “σ “ 

4.	Statistic: The characteristics of a sample are called statistic.
e.g. mean of a sample is denoted as “x̄” 
     standard deviation is denoted as “s”

5.	Variable: A temporary storage where we can store the values.
e.g. x = 5 here, x is called the variable.
 
6.	Experiment: The activity which has a result is called an experiment or survey.
e.g. tossing a coin has a result of head or tail.
The tossing is called the experiment.

7.	Outcome: The result of an experiment is called as an outcome.
e.g. When a coin is tossed, and we get a head.
The head is the outcome of the experiment.

8.	Frequency:  The count of the number of observations in that category or the interval.

9.	Outliers: The values that are inconsistent with data are called outliers.
e.g. if manual labour earns between 10 and 50 maxima but can never earn more than it, but a data shows a person with 1000 as the income that is said to be an outlier.

10.	Extreme Values: The value that are very low or very high are called extreme values. They are not actually outliers as they stay consistent with the remaining part of the data.
e.g.  if any manual labour earns anywhere between 10 to 50 in general. But a person earns 55 then it would be an extreme value.


Sampling Methods

The methods used to select the data from the population.
A sample frame is the elements belonging to a population from which we are extracting the sample.
A sample design is the procedure we use to select the elements from the sample frame.
The selection methods can be of two different types in general:
1.	Probabilistic sampling
The sampling where each observation has an equal probability of selection.
2.	Non-probabilistic sampling
The sampling where observations do not share an equal probability of being a part of the sample.

Probabilistic Sampling
The sampling methods can be further classified into
1.	Simple Random Sampling
In this method of sampling, we randomly select the sample without any procedure associated to the selection.
Advantages: very easy, highly random.
Disadvantages: might not be a right representation of population.

2.	Systematic Sampling
In this method of sampling, we select the sample using a system. Like selection at regular intervals.
e.g. selecting every 10th element in the data.
Advantages: easy, efficient
Disadvantages: if any underlying pattern (cycle or repetitive) exists, it will not be a good method as it will be biased.
For instance, if every 10th observation has diabetes then all the sample will be of diabetic people.

3.	Stratified Sampling
This method first groups the data into strata based on similar characteristics. From each stratum randomly data is selected.
Advantages: reduction in bias.
Disadvantages: prior knowledge in creating the strata.

4.	Quota Sampling
An extension of stratified sampling. It divides the data into strata. Then from each stratum it selects the data in such a proportion as the strata is to the population.
Also called Proportional sampling
e.g. Maths, Science, Social have 30%, 45% and 25% in the population.
From the 3 strata created, of maths 30% is selected, of science 45% and of social 25%.

5.	Cluster Sampling
This method is also an extension of stratified sampling. After the strata is created, it selects samples from only few strata but not all of them.
Advantages: efficiency,
Disadvantages: Sampling and bias errors




TYPES OF DATA
The data can be numerical or categorical in general.

Quantitative (Numerical): The data which is numerical in nature is called as quantitative data. It can be again categorised into discrete and continuous.
Discrete: When the data can take only integer forms. For instance, the count of people born on a day. It cannot be decimal and is finite.
Continuous: The data which can take any value between the interval. For instance, height of a person can lie anywhere in an interval.

Qualitative (Categorical): The data which is in the form of levels is called as qualitative data.
Nominal: The data which do not have an order associated to them. It can be binomial or multinomial.
Binomial is when there are only two categories in the data.
e.g. True/False, 0/1, male/female
Multinomial is when there are more than two categories in the data.
e.g. petrol/ diesel/ gas
Ordinal: The data with categories where the categories have an order associated with them.
e.g. small/ medium/ large

 


DESCRIPTIVE STATISTICS

The data can be described using different measures to understand the data.
They can further classify as 
6.	Measures of central tendency
7.	Measures of dispersion

Measures of Central Tendency
The measures of central tendency describe where the central part of the data lies.

8.	Mean 
The mean is also called the average. It tells us the division point for the data.
It is given as the sum of observations divided by the number of observations.

Mean = sum of observations / number of observations

It is a calculated field.
Mean is very sensitive to the extreme values and is not considered a best metric to understand the data.

13, 18, 13, 14, 13, 16, 14, 21, 13
Mean = 13+18+13+14+13+16+14+21+13 / 9   = 15


9.	Median
The median is the middle most value in the distribution of the data.

Sort the data in ascending order
If number of observations is odd, 
Median = n+1/2 th observation
If number of observations is even.
Median = average of n/2 th observation and n/2 +1 th observation

13, 18, 13, 14, 13, 16, 14, 21, 13
13, 13, 13, 13, 14, 14, 16, 18, 21
N = 9
Median = 9+1/2 = 5th observation = 14

It is a positional field.
Median is also subject to outliers or extreme values. It is affected by extreme values but not as much as the mean. Hence is a better metric than the mean in situations where mean is not a good metric.


10.	Mode
The most frequent value in the data is called as mode. It is a metric used for categorical features. It is not usually considered in case of numerical features.
Unimodal: The data with only one mode
Bimodal: The data with two modes
Multimodal: The data with more than two modes

13, 18, 13, 14, 13, 16, 14, 21, 13
13 – 4
14 – 2
16 – 1
18 – 1
21 – 1
Mode = 13

It is neither calculated nor a positional field.
Mode is not subject to outliers or extreme values. It is not affected by extreme values like mean or median.

Measures of dispersion
The measures of dispersion describe the spread of data that is it helps understand how the data is distributed

11.	Range
The range is the difference between minimum and the maximum values in the data.

Range = Maximum – Minimum

13, 18, 13, 14, 13, 16, 14, 21, 13
Range = 21-13 = 7

It is affected by outliers in the data. Hence is not considered a good measure for understanding the data.

12.	Deviation
The difference between the observed value and the estimate of the location usually the mean. They are also called as Errors or Residuals.

Deviation = Observed value – Estimate

13, 18, 13, 14, 13, 16, 14, 21, 13
Mean = 15
13 - 15 = -2
14 – 15 = -1
16 – 15 =1
18 – 15 =3
21 – 15 =6

13.	Standard deviation
This measure how deviated the observations are from the mean and from each other.

Standard deviation of population:
 


Statistical deviation of sample:
 

Standard deviation is also affected by the outliers. Since it calculated the deviations which are also affected by the outliers.


We use n-1 to calculate for sample measures rather than n to account for the degrees of freedom. Using n with undercalculate the statistic but with n-1 will be a better explanation. The degrees of freedom are the number of observations which can be varied that is which can be moved freely. N-1 accounts to the observations that can move freely as one observation is kept constant.


1.	Variance:
The variance is also a spread of the data. It tells us on an average how deviated are the data points from the mean.

Variance = standard deviation ^ 2


2.	Quartile:
The data when divided into 4 equal parts gives us the quartiles. It is one of the measures of calculating the extreme values in the data. Ever quartile has equal number of observations. They contain 25% of the observations.

1st quartile = n+1/4 th observation
2nd quartile = Median = n+1/2 th observation
3rd quartile = 3(n+1)/4 th observation.


3.	Inter quartile range
The interquartile range is the difference between the third and the first quartiles. It tells us where the 50% of the data lies. 

IQR = 3rd quartile – 1st quartile

It is considered as one of the methods to remove the extreme values in the data.
It is given as 

Lower limit = 1st quartile – 1.5*IQR
Upper limit = 3rd quantile + 1.5*IQR

Any value lower than lower limits or any value greater than the upper limit is considered as outliers.

4.	Skewness
The skewness is the measure of the asymmetry of the data.
Any data can have different kinds of distributions like normal, binomial etc.
In case of normal distribution, the skewness = 0 since there symmetry around the mean.

Skewness = 3(Mean-Median) / standard deviation

Skewness can be of two types:
Right skewness / Positive skewness:
skewness>0
Mean > Median >Mode
It happens when there are few extreme values on the right tail of the data. 
Left skewness / Negative skewness:
Skewness<0
Mean< Median< Mode
It happens when there are few extreme values on the left side of the data

No skewness:
Skewness =0
Mean = Median = Mode
It happens when data is normally distributed


14.	Kurtosis
It is a measure of tailedness or the peakedness in the data. It tells us what kind of distribution the data has.

Positive kurt: Leptokurtic:
Kurt >3
Excess kurt >0
Excess kurt =kurt -3
When the data is leptokurtic then the data lies very near to the mean or in other words, the standard deviation is low. 
Lepto means skinny and the distribution looks like a long peak.
It indicates that the extreme values or outliers are large.

Mesokurtic: No kurt:
Kurt = 3
Excess kurt =0
When the data is mesokurtic then the data lies symmetric around the mean, in other words it is normally distributed.
It indicates that there are no outliers or extreme values in the data

	Platykurtic: Negative kurt:
	Kurt <3
	Excess kurt <0
When the data is platykurtic then the data lies far from the mean, in other words the standard deviation is high.
Platy means broad and hence distribution looks like a broad distribution.
It indicates that the extreme values or outliers are small.


15.	Covariance
The covariance is a measure of direction of movement of the variable in respect to each other.
 
It only tells us the direction of movement of the variables with each other
It is not interpretable.
It can be positive or negative.
When covariance >0 then with an increase in one variable there will be an increase in the other variable
When covariance <0 then with increase in one variable there will be a decrease in the other variable


16.	Correlation
Also called the coefficient of covariance
This is a measure of both the direction and the magnitude of the movement of the variables in respect of each other.

 

Correlation is preferred to covariance as it is interpretable.
It always lies between -1 and 1
If correlation =0 then there is no relation between the variables
If correlation =1 then with a unit increase in one variable there is a unit increase in another variable.
If correlation =-1 then with a unit increase in one variable there is a unit decrease in another variable.


Correlation does not mean causation.
Causation means an evet that happens because another event happens that is it is a pre-established relationship.
Correlation only implies statistically they move but not as a cause is involved.


 

DATA VSUALISATION
The visualisation of any data will help uncover better patterns in the data. And for any person visualisation is a better technique to understand the data.

11.	Histogram
The plot shows the distribution of the data which is numerical in nature.
It plots the intervals against their distributions.
The bins are of equal width. 
Number of bins is dependent on the user.
The height of the bin is the frequency.
x-axis = interval
y-axis = frequency
	

2
14
14
14
16	18
20
20
21
23	27
27
27
29
31	31
32
32
34
36	40
40
40
40
40	42
51
56
60
65

	Step1: calculate range
	Range = 65-12=53
	
	Step2: Divide range into number of groups and round up
	n=6
	
	53/6 = 8.8 ~9

	Step3: Use class width to create the groups

	
 

Classes	Frequency
12-21	8
21-30	6
30-39	6
39-48	6
48-57	2
57-66	2


	 


	
 
5.	Bar plots
The plots that show the distribution of a categorical variable. It plots the frequency against the category.
X – axis = category
Y – axis = frequency


Category	Frequency
G1	1
G2	2
G3	3
G4	4
G5	5

 

 
6.	Pie charts
The pie charts are circular graphs that show the distribution of the categories in the variable based on their percentages.
It plots the percentage of total observations for each category.
	There are no axes to the chart
	100% = 360 degrees in a pie chart
	Sum of all the observation frequency percentages is 100%.

Fruit	Percentage
Peach	10
Orange	13
Pineapple	20
Grapes	27
Banana	30
	






	 


7.	Box plots
One of the plots used to view the numerical data. It is called the box and whiskers plot.
It is called as 5-summary plot
It includes:
Lower limit
1st quartile
Median
3rd quartile
Upper limit

 

If the minimum and maximum values lie below the limits of the IQR range, then we cannot see the points after the whiskers (lines) in the plot.
But if the values lie above and below the limits, we can use this to see how they are distributed. In such case minimum value = least value point and maximum value = highest point in the graph.
8.	Scatter plots
The graph shows the relationship between the two continuous features. It helps us understand how two features are related to each other.

X – axis = one variable
Y – axis = another variable

 
