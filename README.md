# Handwritten Number Detector ✍️✍️
📝📝 Description:
This project delves into the world of digit recognition using the MNIST dataset, a classic in computer vision. The goal was to develop models capable of accurately identifying handwritten digits. My initial thought was to use a logistic regression but having 70,000 examples felt like it would be a waste and then tried a deep neural network with 100 hidden layers which provided better predictions.
 
## Dataset 🗃️🗃️
The dataset was imported from the sklearn.datasets library with 70,000 training examples and 10,000 testing examples.
mnist = fetch_openml('mnist_784')

## Geeky specs
The model uses the adam optimizer because it combines elements of two other popular optimizers: RMSprop and AdaGrad, to provide an efficient and effective optimization technique. 
Since this model has multi-class classification problems where the labels are integers as the prediction outputs sparse categorical crossentropy was used as the loss function.
There is a hidden layer with 100 neurons in the model with the relu activation function and the input and the input and output layers are fit with the sigmoid activation function.

## Models 💻💻 
The accuracies on the testing set of the models I used are the following
Logistic Regression: 92.58%
Neural Network : 92.54%
Deep Neural Network : 97.46% 
