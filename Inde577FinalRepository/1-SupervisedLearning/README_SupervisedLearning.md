# Supervised Learning

Supervised learning is a type of machine learning model where the model is trained on a labeled dataset, where each datapoint in the training dataset is paired with an output label which the model is trying to predict. Essentially, supervised learning uses existing data points to build a predictive model on unseen pairs of data. The image below illustrates a high level description of Supervised Machine Learning:

![Alt text](image.png)

As we can see, each data $\mathscr{x_i}$ is paired with a label $\mathscr{y}$ through a target function $\mathscr{f}$ which is unknown. Our goal in supervised learning is to approximate this function to the best of our ability.

**Part 1: Learning**

Outlined below is a general framework that all Supervised Machine Learning models follow in creating this association function $\mathscr{f}$

![Alt text](image2.png)

Essentially, we are given existing data ($x_1$, $y_1$),...,($x_N$, $y_N$) which becomes our **training** data set. Our Learning Algorithm $\mathscr{A}$ looks to identify a function $\mathscr{g}$ from our Hypothesis Set $\mathscr{H}$ of possible functions that best approximates our true association function $\mathscr{f}$. The Learning Algorithm $\mathscr{A}$ differs across various Supervised Learning Models (which we'll see as we explore different models), but this overall framework is consistent across Supervised Learning models.

**Part 2: Measuring Model Performance**

In order for our Learning Algorithm $\mathscr{A}$ to pick an optimal model from our hypothesis test, we develop a function that measures how well a hypothesized model $\mathscr{g}$ fits our data. The most natural way to do this is through a loss function: 

$ L = \eta \sum_{i=1}^{N} (g(x^{(i)}) - f(x^{(i)}))^2 $

where N is the number of samples and $\eta$ is a positive scalar or a function of N. Our best fit model $\mathscr{g}$ would be when our loss function $\mathscr{L}$ is minimized.

## Types of Supervised Learning Models
There are several types of Supervised Machine Learning Models, and each one has two characteristics:

Characteristic 1: Parametric vs Non-Parametric
- Parametric models have a fixed number of parameters determined during the training process (Ex: Linear, Logistic, Neural Networks)
- Non-parametric models learn directly from the data with no assumptions about the number of parameters (Ex: Decision Trees, random forest models, K-Nearest-Neighbors)

Characteristic 2: Classification vs. Regression:
- Classification Models predict a class/category that data belongs to (logistic regression, Decision Trees, K-Nearest-Neighbors)
- Regression Models predict continuous numerical variable data (Ex: linear regression, polynomial, neural networks)




