### Description of the Code

The provided code implements polynomial regression from scratch using Python and the NumPy library. Below is a detailed description of each part of the code:

1. **Importing Libraries**:
    - The `numpy` library is used for numerical computations, and `matplotlib.pyplot` is imported for plotting purposes.

2. **Global Variable**:
    - A global list `losses` is initialized to store the loss values during training.

3. **Loss Function**:
    - This function computes the Mean Squared Error (MSE) between the true and predicted values.

4. **Calculate Gradients**:
    - This function calculates the gradients of the loss function with respect to the weights and bias.

5. **Create Polynomial Feature Set**:

    - This function creates polynomial features by raising the input features to the specified degrees and appending them to the original feature set.

6. **Training Function**:

    - The `train` function implements the training process using batch gradient descent. It updates the weights and bias over multiple epochs and records the loss at each epoch.

7. **Prediction Function**:

    - The `predict` function uses the trained weights and bias to make predictions on new input data.

8. **R² Score Calculation**:

    - This function computes the R² score to evaluate the performance of the regression model. The R² score indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.

