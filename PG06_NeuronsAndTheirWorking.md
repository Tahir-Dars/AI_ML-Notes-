# What are Neurons ?
In machine learning, neurons refer to the basic units of computation within artificial neural networks (ANNs),
inspired by biological neurons in the human brain. Each neuron receives one or more inputs, processes them, 
and produces an output.
Neurons are organized into layers within a neural network:

### Input Layer
 Neurons receive input data.
### Hidden Layers
 Intermediate layers between the input and output layers where complex computations occur.
### Output Layer
 Neurons provide the final output of the network.
# How Neurons Work
When we provide many input examples in the form of data and labels, an AI model learns to match the data to the
labels and discovers patterns within the data. This technique, known as machine learning, involves learning from
examples and pattern recognition.There are numerous approaches to machine learning, but one frequently used tool
is the neural network, which consists of a network of artificial neurons.Imagine you have an input, X, and you 
need to predict an output, Y, such that there is a specific relationship between X and Y. For instance, X could 
represent the square footage of a house, and Y could represent the price of the house. In this case, the 
relationship between X and Y is defined by the following equation:
### Y=2X−1
![xandy](https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/0de0d252-d442-432e-8a37-bb32c22028be)
You get the slope line in blue in Figure 2.2.1 when you join all the points (X, Y) plotted on the graph. Due to the
specific relationship between X and Y, when X is -2, Y is -5, and when X is 3, Y is 5.The relationship between X and
Y can be considered a function, where applying the function to X results in Y.
## Artificial Neuron
An artificial neuron is essentially a mathematical function that converts numerical inputs into numerical outputs 
using learnable parameters called weights and biases.

![Single AN](https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/a539380d-53f1-408e-9c98-3b7ff490b23d)
_____________________________________________
#  Key Concepts
  ##  Function
A function is an expression that defines the relationship between an input and an output. The following function 
calculates Y based on the input X. Y is the value returned by the function.
#### Calculate Y (X){
#### Y = W*X + B;
#### return Y }
  ## Parameters
Parameters are values provided to functions that determine their output. The following function takes X, W, and B
as parameters to calculate Y. Here, X is the known input, and the model uses X along with W and B to compute the output.
#### Calculate Y (X){
#### Y = W*X + B;
#### return Y }
## Artificial Neuron
An artificial neuron is a mathematical function that takes in inputs and parameters and calculates an output. 
The power of neural networks results from a vast number of artificial neurons networked together.
## The Learning in Machine Learning
Given the equation Y = 2X - 1, we can calculate values of Y for different values of X, knowing W is 2 and B is -1. 
If we provide these values as training data to a machine, it learns the parameters W and B to predict the output 
for new, unseen values of X.

<img width="189" alt="table01" src="https://github.com/Tahir-Dars/AI_ML-Notes-/assets/150343129/2ab301da-7f37-4e3b-98b8-6dc80b4484bb">

## Learning Steps 
#### .  The machine starts with random guesses for W and B and calculates the error (loss) based on the predicted and actual Y values.
#### .  It adjusts W and B to minimize this loss iteratively, generating new guesses.
#### .  For example, initial guesses with large errors are refined to produce reduced errors.
#### .  This process continues until optimal parameters are found, which are then tested with new inputs for accuracy.

Based on the Learning Steps, we can conclude that machines learn by figuring out a pattern or a relationship by guessing the parameters, calculating the loss, and using this information to generate new and better guesses. 

















