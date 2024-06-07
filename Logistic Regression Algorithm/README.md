### Description of the Code

The provided code implements a logistic regression model from scratch using Python and the NumPy library. Below is a detailed description of each part of the code:

1. **Sigmoid Function**: This function computes the sigmoid of an input array. The sigmoid function is used to map any real-valued number into the range [0, 1].

2. **Logistic Regression Class**: This class encapsulates the logistic regression model.

    - **Initialization**: The constructor initializes the learning rate, number of iterations, and model parameters (weights and bias).

    - **Model Training (fit method)**: The `fit` method trains the model using gradient descent. It iteratively updates the weights and bias based on the gradients of the loss function with respect to the model parameters.

    - **Prediction (predict method)**: The `predict` method computes the class labels for input data by applying the sigmoid function to the linear predictions and then thresholding the output at 0.5 to obtain binary class labels (0 or 1).

