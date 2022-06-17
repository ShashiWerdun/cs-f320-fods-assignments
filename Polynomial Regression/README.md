# Polynomial Regression

## Model Description
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

## Results
At the time of writing this code, fixing the number of iterations and learning parameter:
- 3rd degree polynomial yields the best model without any regularization
- Regularizing the models showed very marginal improvement in training and testing errors.

<img src="./Plots/Gradient%20Descent%20Results/GD%20Degree-3.png">