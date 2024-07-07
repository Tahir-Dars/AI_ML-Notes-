# The Machine Learning Process
In the previous lesson, we learned how machines find the correct parameters for the relationship between input X and output Y, defined by:Y=W∗X+B
The machine starts with random values for W and B, then measures how far its predictions are from the actual values using a loss function. It 
then optimizes these guesses to reduce the loss. This process repeats until the loss is minimized.

![ML process](https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/52bf2d60-cc3f-4179-afce-49143c9dc11b)
Remember, the input value X is provided to the computer along with the target value. The computer creates a model that predicts output value Y 
using learnable parameters W and B.
# Understanding Loss and Optimization
To understand loss and optimization, let’s consider that the model starts by assigning the value 10 to W and B. Now refer to Tablegiven below and examine the guess values and the error values. 

**Note:**

**The “guess” is the predicted output value for a given value of X with parameters W and B (both set at 10).** 

**The “error” is the difference between the guess and the actual Y value.**

<img width="195" alt="table02" src="https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/831d60fa-704e-43ba-a3e7-02bbc1a0211e">

To get a good idea of the total loss, calculate the average of all errors. To avoid positive and negative errors canceling each other out, use the squares of the errors. The average of the sum of squared errors is often used as the cost function.

<img width="219" alt="table03" src="https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/de9f15b1-42a5-44f8-b603-553e1399d339">

In the previous lesson, plotting Y against X gave a linear graph. Plotting the loss function against a parameter (W or B) gives a parabolic graph.

<img width="514" alt="tables" src="https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/eaac547b-65ca-4f93-b746-1498c303f4d4">

In Figure above , point A represents the initial loss function value with random W and B. The gradient at this point indicates the direction
 towards the lowest error. The optimizer adjusts W and B based on this gradient, incrementally moving closer to the minimum error (Figure Upper ).
 The step size is determined by the learning rate, set by the programmer. Too low a learning rate prolongs convergence, while too high can overshoot the minimum.
Gradient Descent is the process of descending along the loss curve to minimize error. With multiple parameters, such as W and B, more complex graphs
 are used, but the fundamental concept of gradient descent remains unchanged.
________________________________________________________________________________________________________________________________________________________________________________
# Key Concepts 
## Loss Function
The loss or cost function measures how well a model predicts the output from a given input. In the example discussed in this lesson, the loss or
cost is calculated as follows: The error for each example is calculated by subtracting the actual or ground-truth value (Y) from the predicted
value and squared to remove negative values. The squares of all the errors from the dataset are added, and the mean squared error is calculated.

## Optimization

Optimization is a method by which a model adjusts the parameters (W and B) based on the loss value obtained during each iteration. In the example
discussed in this lesson, the model optimizes the parameters by adjusting the parameters such that the cost moves towards the minimum possible value.

## Gradient Descent

During optimization, the model’s algorithm looks at the slope of the loss or cost function calculated at a point in time. The parameters (W and B) 
are adjusted based on the slope or gradient of the cost function curve (plotted on the y-axis with the parameters on the x-axis). The net result of 
this tuning is that the cost function descends in the direction of the minimum possible cost value. This optimization calculation is called gradient 
descent and involves the use of calculus.

## Learning Rate

The learning rate determines the step size of the cost function during gradient descent. A lower learning rate leads to a more gradual descent, while 
a larger learning rate leads to more rapid gradient descent.

## Training Set

The training set refers to the portion of data you use when making your guess, measuring the loss, and using calculus to move down the curve to make a 
more accurate guess. The model uses the training set to find the optimal parameters W and B that minimize the cost or loss for the model’s prediction.

## Testing Set

The testing set is the portion of data used to gauge a model’s final accuracy. Unlike the training data, which has labeled inputs (the actual outputs 
are provided for each input for each example), the testing data inputs do not have labels or outputs. This is data that a model has never seen and is 
used as a final test for the model.

