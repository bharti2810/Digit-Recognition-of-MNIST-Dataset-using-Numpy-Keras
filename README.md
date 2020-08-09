# Digit-Recognition-of-MNIST-Dataset-using-Numpy-Keras
Building fully operational Neural Network using NumPy and Keras and compared their performances. The steps followed to build the network 
- feedforward
- loss computation
- backpropagation
- weight updates etc.

* There are functions assigned to different subparts of feedforward.

* The whole data is taken as one batch. No minibatch gradient descent is performed
* The cumulative input to the layer Z<sub>l</sub>  is now a step in feedforward
* The output of the last layer is denoted as H<sub>L</sub> .There are L−1 hidden layers.
* For each layer l, the Z<sub>l</sub> is stored as 'activation_memory' and H<sub>l−1</sub>W<sub>l</sub>,b<sub>l are stored as 'linear_memory' to use later in backpropagation
 
