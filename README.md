# Mobile Price Classification Project

This project builds and trains an artificial neural network (ANN) model to classify mobile phones into different price ranges based on their features.

## Data

The dataset used is the [Mobile Price Classification dataset](https://www.kaggle.com/datasets/iabhishekofficial/mobile-price-classification) from Kaggle. It contains 2000 observations of mobile phones with various features like battery power, clock speed, RAM etc. along with a target price_range variable.

The data is split into 75% training and 25% testing sets.

## Model

The model architecture consists of:

- Input layer with 21 input features 
- Hidden layer with 8 neurons and ReLU activation
- Hidden layer with 4 neurons and ReLU activation  
- Output layer with 1 neuron and sigmoid activation (for binary classification)

The model is compiled with Adam optimizer, binary cross-entropy loss and accuracy metric.

It is trained for 100 epochs with a batch size of 32.

## Usage

The model can be retrained by running the Jupyter notebook. The final model weights are saved to `mobile_price_ann_weights.h5`. This can be loaded to make predictions on new data.

## Contributing

Pull requests are welcome for improving the model accuracy or adding new features like model exports.
