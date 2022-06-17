# Implementing ML algorithms from scratch

This repository implements [polynomial regression](./Polynomial%20Regression) using gradient descent and stochastic gradient descent and [feature selection](./Feature%20Selection/) using greedy forward and greedy backward selection without the use of popular machine learning libraries like scikit learn.

## Polynomial Regression

### Model Description
With the help of provided code, we can produce 6 different types of
models varying in the algorithm they use -
1. Gradient Descent without Regularization.
2. Gradient Descent with Lasso(L1) regularization.
3. Gradient Descent with Ridge(L2) regularization.
4. Stochastic Gradient Descent without Regularization.
5. Stochastic Gradient Descent with Lasso(L1) regularization.
6. Stochastic Gradient Descent with Ridge(L2) regularization.

This is done using appropriate arguments to the functions present in the code.
To understand more about the algorithm implementation, check out this [doc](./Polynomial%20Regression/Assignment1_Polynomial_Regression.pdf).

## Feature Selection

### Model Description
The code provided under [feature selection](./Feature%20Selection/) performs different pre-processing techniques and produces the best subset of features out of the given features list using greedy forward and greedy backward methods.
#### Pre-processing techiques: 
- Replaced all the Nan values in the data with the mean value of the
respective column
- Normalized the data using z-score normalization
#### More about feature selection:
Here we consider generating all the possible subsets and determine the subset with the least error but this is computationally expensive so we consider 2 greedy approaches: 
- **Greedy Forward Selection**: In each iteration, we consider the previous iteration best feature set and see which feature of the remaining ones will yield minimum error.
- **Greedy Backward Selection**: We can initially consider all the features as reliable and keep on deleting the feature that is currently the least reliable.<br><br>
**<u>Note</u>**: In both approaches, we used gradient descent with no
regularization for estimating the linear regression models in each iteration.
