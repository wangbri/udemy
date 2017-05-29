# Section 3
## Linear Regression
*using (ml_linear_cost_example.ipynb)*

Use squared error loss function to determine accuracy of linear regression hypothesis. Objective is to find the weights associated with the linear regression equation.

__numpy.random.rand(150)*20__ generates a series of random values from [0, 1) by default and can be specified to return 150 random values between 0 and 20 in this case. This series can serve as x values for a given function to calculate our training set.

To find the correct weight, linear regression uses a loss function to determine how close or far the predicted value is from the actual. Loss is 0 when predicted value is exactly equal to the actual value.

**np.linspace(3,7,100)** generates 100 evenly spaced values between 3 and 7. This series can serve as weights to be used to generate a series of predicted y values with each of the weights.

## Gradient Descent
Squared error loss/cost function is used to find the predicted loss at each of the weights and derivative at a particular weight can be used to see which weight value to gravitate towards to get the minimum loss for the function. For linear regression, loss functions will have a global optima or minimum cost.

Large learning rates can lead to iterations oscillating between larger and larger values in the loss function and diverging towards infinity. Small learning rates will cause the optimization to take several small iterations before converging at the minimum.

AWS's machine learning service will automatically test several different learning rates to find the best one for the function and add it to the logs.

There are two types of gradient descent:
- **Batch gradient descent** computes the loss between predicted and expected values of y for all examples in the training set to create the loss function. Weights are adjusted based on the loss function after the loss function is created. Computation step in creating the loss function will be resource-intensive and slow if the training set is large.

- **Stochastic gradient descent** computes the loss between the next training example and adjusts the weights iteratively for each of the examples in the training set. Convergence will occur more quickly if the training set is large but if the training example is not shuffled or ordered by some feature, it will result in suboptimal weights. The training algorithm might adjust the weights to accommodate a specific cluster or group of training examples. And then when it encounters a different type of training example, the algorithm would have to adjust the weight by a large amount but it might not be able to do so because the differences would be too big.

AWS's machine learning service uses stochastic gradient descent for its learning method.

Hyperparameters are parameters that are predetermined before the model-building step such as the learning rate in this case. These parameters cannot be determined from the training data.
