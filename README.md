# Digit-Recognition-of-MNIST-Dataset-using-Numpy-Keras
Building fully operational Neural Network using NumPy and Keras and compared their performances. The steps followed to build the network 
- feedforward
- loss computation
- backpropagation
- weight updates etc.
-------------------------------------------------

# Data Preparation
- Firstly, we load the data using the function load_data(). The function data_wrapper() is then applied to the data to get the train and test data in the desired shape. Please note that the code needs to take a batch of data points as the input. Hence, be careful while checking the dimensions.
- we have 28x28 greyscale images in the MNIST dataset. Hence, each input image is a vector of length 784. The ground truth labels of a batch are stored in a matrix which is converted to a one-hot matrix. Also, the output of the model is a softmax output of length 10. 
 

* There are functions assigned to different subparts of feedforward. The whole data is taken as one batch. No minibatch gradient descent is performed. The cumulative input to the layer Z<sub>l</sub>  is now a step in feedforward. The output of the last layer is denoted as H<sub>L</sub> .There are L−1 hidden layers. For each layer l, the Z<sub>l</sub> is stored as 'activation_memory' and H<sub>l−1</sub>W<sub>l</sub>,b<sub>l</sub> are stored as 'linear_memory' to use later in backpropagation.

changes mentioned above:
H<sub>0</sub>=B
for l in [1,2,.......,L−1]:
	Z<sub>l</sub>=Wl.H<sub>l−1</sub>+bl
	Hl=σ(Z<sub>l</sub>)
	HL = softmax(WL.H<sub>L−1</sub>+b<sub>L</sub>)



