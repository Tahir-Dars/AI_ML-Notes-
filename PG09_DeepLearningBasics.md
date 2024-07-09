# Deep Learning 
Deep learning is a subset of machine learning that involves neural networks with multiple layers (often referred to as deep neural networks) to model and understand complex patterns in large amounts of data. It uses algorithms inspired by the structure and function of the brain's neural networks to learn from data in a hierarchical manner, automatically extracting features and representations without manual intervention. This approach enables deep learning models to achieve high accuracy in tasks such as image and speech recognition, natural language processing, and autonomous systems.
## Weights and Biases
 we learned that an artificial neuron is a mathematical function that converts numerical inputs into numerical outputs using learnable parameters called weights and biases. 

 ![WandB](https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/aad6b3e4-c808-4b0c-9f2b-431de197b943)

## Dense Networks
Artificial neurons are arranged in a series of connected layers to form an Artificial Neural Network (Refer to Figure below). Within each layer, neurons are grouped vertically. Information flows sequentially from the left side of the network to the right. Notably, each neuron in the first layer is connected to every neuron in the second layer. Similarly, each neuron in the second layer is fully connected to all neurons in the third layer. Networks with such fully connected structures, as illustrated in Figure below, are known as Dense Networks.

![Xs and Ys](https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/3c7aa9a7-aaeb-40c7-b3a2-0ebb64f1f98d)


![dogsAndcats](https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/f354931b-c1cc-466a-a2bc-52e5fec1fab0)


Consider a model designed to classify images as either cats or dogs, where the input is provided in the form of pixel data. As shown in the Figure below, the neural network comprises two layers: the first layer contains three neurons, and the second layer consists of two neurons. Each neuron in the network receives input, processes it, and outputs a value that is then passed to a neuron in the subsequent layer. The output is computed using the learnable parameters W (weights) and B (biases). The model optimizes these parameters during the learning process as follows:

**1.The neuron initially estimates the values of the parameters.**

**2.The model evaluates the accuracy of this estimation by calculating the loss or cost.**

**3.The parameters are then optimized and updated to improve the model's performance.**

This process happens in each neuron across the entire network until the network works as intended. 

The model we are discussing should provide an output that represents either a dog or a cat. Since outputs need to be numerical, data is labeled using one-hot-encoding to label classes using 1s or 0s. In the example shown in Figure above, there are two neurons in the final layer; each one outputs a number. The output (1, 0) from these two neurons represents a cat, while (0, 1) represents a dog. 
Remember that real-life models will usually need thousands of neurons to classify image data. 

**Recognizing Handwritten Digits**

Now, consider a model designed to recognize and classify handwritten numeric digits. Unlike the Neural Network: Example model discussed in Part 1, which had two possible outputs (cats or dogs), this model has ten possible outputs, corresponding to the digits 0 through 9. This expanded range of classifications allows the model to identify each individual digit accurately, making it a more complex and versatile application of neural network technology.

![0and1](https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/c45998f5-02f3-48b5-a56f-512f10a31b85)

**One-hot-encoding for Numeric Digits**

Since we have ten categories of outputs, we label the data with an array of 10 numbers, with the appropriate array item being a 1 and the remaining 0 (Refer to Figure above). 

The data consists of 70,000 images of handwritten digits (Refer to Figure above), with 7000 images for each digit. This data set is split into a training set of 60,000 images and a testing set of 10,000 images. Each image is a greyscale 28x28 pixel image, i.e., with 784 pixels.

<img width="356" alt="1,0and7" src="https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/55a2aad5-dae2-40fc-a455-dfb3f5607a4a">

## How the Model Works

![modelworking](https://github.com/Tahir-Dars/AI_ML_Basics--Notes-/assets/150343129/f3864615-79b5-4041-827e-f479e4a9d25d)

The 784 pixels of each image are fed as numerical inputs to the first layer, which consists of 20 neurons (Refer to Figure below). The model is also instructed that if the input represents a digit 7, the output neurons should all produce a value of 0, except for the one representing 7, which should output 1. The model is trained using these input training data (pixel values of images) and their corresponding labels.

## During training

Each neuron initially estimates the parameters that will yield the desired output.
The model evaluates the accuracy of these estimations, measuring how correct or incorrect the guesses were, and then optimizes the parameters accordingly.
Each neuron determines the optimal weights and biases that will produce the correct output, either for the next layer or as the final answer (if the neuron is in the last layer).
Over time, these estimations are continually measured, optimized, and updated, enabling the network to accurately recognize handwritten digits.

___________________________________________________________________________________________________
# Key Concepts

## Deep Learning
A machine learning technique involving artificial neurons arranged in networks consisting of multiple layers such that learning happens across each layer and in each neuron.

## Artificial Neural Network
A network of connected neurons, arranged in vertical groups called layers, in which information flows in one direction from input to output.

## Dense Neural Networks
A type of neural network in which a layer's neurons are connected to every neuron of the next layer.

## One-hot-encoding
A way of labeling categories using 0s and 1s; each category is represented by an array of 0s and 1s, with a single 1 in a distinct position while the rest are 0s.

































