# Feature Selection

## Model Description
The code provided under [feature selection](./Feature%20Selection/) performs different pre-processing techniques and produces the best subset of features out of the given features list using greedy forward and greedy backward methods.
### Pre-processing techiques: 
- Replaced all the Nan values in the data with the mean value of the
respective column
- Normalized the data using z-score normalization
### More about feature selection:
Here we consider generating all the possible subsets and determine the subset with the least error but this is computationally expensive so we consider 2 greedy approaches: 
- **Greedy Forward Selection**: In each iteration, we consider the previous iteration best feature set and see which feature of the remaining ones will yield minimum error.
- **Greedy Backward Selection**: We can initially consider all the features as reliable and keep on deleting the feature that is currently the least reliable.<br><br>
**<u>Note</u>**: In both approaches, we used gradient descent with no
regularization for estimating the linear regression models in each iteration.

## Results
Check out this [doc](./Results/Report.pdf) for the training and testing errors with best feature set generated.