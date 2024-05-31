# MNIST Digit Classification with Convolutional Neural Network
This project trains a Convolutional Neuarl Network (CNN) ti classify handwritten digits from the MNIST dataset. The model is built using TensorFlow and Keras libraries. 

## Project Description 
The objective of this project is to bulid and train CNN that can accurately classify handwritten digits (0 - 9) from MNIST dataset. 
The MNIST dataset contains 60,000 training images and 10,000 testing images. 

## Usage 
1. Loading MNIST dataset: The dataset is loaded and divided into training and testing datasets.
2. Pre-processing: The data is normalized to have values between 0 and 1.
3. Reshaping: The images are reshaped to fit the input shape required by the CNN.
4. Model Training: The CNN model is built and trained on the training dataset.
5. Evaluation: The model's performance is evaluated on the test dataset.
6. Prediction: The model can be used to predict digits from new images.

## Models Architecture 
The CNN model consists of following layers:

1. Conv2D Layer: 64 filters, kernel size 3x3, ReLU activation, max pooling with pool size 2x2.
2. Conv2D Layer: 32 filters, kernel size 3x3, ReLU activation, max pooling with pool size 2x2.
3. Conv2D Layer: 16 filters, kernel size 3x3, ReLU activation, max pooling with pool size 2x2.
4. Flatten Layer: Converts the 2D matrix data to a vector.
5. Dense Layer: 64 units, ReLU activation.
6. Dense Layer: 32 units, ReLU activation.
7. Dense Layer: 10 units, Softmax activation (output layer).

## Evaluation
The model is trained for 5 epochs and evaluated on the test dataset. The performance metrics include loss and accuracy.

## Prediciton and Custom Image
The model can also be used to predict digits from custom images. For example, given an image of a handwritten digit, the script will preprocess the image and use the trained model to predict the digit. 