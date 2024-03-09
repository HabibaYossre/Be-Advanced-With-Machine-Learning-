# *Linear Regression from Scratch :*

### Linear Regression is a fundamental and widely used statistical method in machine learning and statistics for modeling the relationship between a `dependent variable` (target) and one or more `independent variables` (features). 

**There are two main types of linear regression:**

* *Simple linear regression* uses only one independent variable.
* *Multiple linear regression* uses two or more independent variables.
---
#### ***1) Model Representation:***

The basic idea is to represent the relationship between the variables as a linear equation.
For a simple linear regression with one independent variable: **y=mx+b**
where 

* **`y`** is the dependent variable, 

* **`x`** is the independent variable, 

* **`m`** is the slope, and 

* **`b`** is the y-intercept.

![alt text](<images/Hypo Function.png>)


----

#### ***2) Objective Function (Cost Function):***

* The goal of linear regression is to find the parameters (slope and intercept) that minimize the difference between the predicted values and the actual values.

* This is achieved by defining a cost function (also known as the objective function) that measures the difference between predicted and actual values. 

![alt text](<images/Cost Function jpeg.jpeg>)

- **MSE function can be calculated as:**
   
   ![alt text](<images/Cost Function formula.jpeg>)

    where: 

  * `h(x)` is the predicted value, 
  * `y` is the actual value, 
  * `m` is the number of training examples, and 
  * `θ` represents the parameters.
----
#### **Gradient Descent:**

* A linear regression model can be trained using the **optimization algorithm gradient descent** by iteratively modifying the model’s parameters to reduce the mean squared error (MSE) of the model on a training dataset. To update θ1 and θ2 values in order to reduce the Cost function (minimizing RMSE value) and achieve the best-fit line the model.

* Gradient descent iteratively updates the parameters in the direction of the steepest decrease in the cost function.

* The update rule for gradient descent is given by:

![alt text](<images/gradiant_descent (slope).jpg>)

**Now, let's break it down:**
**1) θ:** This represents the parameters of the function that we are trying to optimize. In the context of machine learning, θ often represents the weights of a model.

**2) α:** This is the learning rate. It's a small positive number that determines the size of the steps we take during each iteration. Choosing the right learning rate is crucial, as too small a value can make the algorithm slow, while too large a value may cause it to overshoot the minimum.

**3) J(θ):** This is the cost or loss function, which measures how well our model is performing. The goal is to minimize this function.


**4) ∇J(θ):** This is the gradient of the cost function with respect to the parameters 

**Explanation:**

**1.** We start with an initial guess for `θ`.
**2.** Compute the gradient `∇J(θ)`, which indicates the direction of the steepest increase of the cost function.
**3.** Update θ by moving in the opposite direction of the gradient, scaled by the `learning rate α`.
**4.** Repeat this process until `J(θ)` converges to a minimum.

*In simple terms*, gradient descent is like descending a mountain by taking steps in the steepest downhill direction. The learning rate controls how big each step is, and the process continues until you reach the lowest point (minimum) of the mountain (minimum of the cost function).


![alt text](<images/gradiant_descent .jpg>)

----
#### Summery:

| *Function* | *Objective* |
|----|----|
|**Hypothesis Function**|often denoted as ℎθ(x), calculates the predicted output by multiplying each input feature by a corresponding weight and summing them up.|
|**Cost Function**|typically represented as J(θ), quantifies the error between predicted and actual values, aiming to minimize this error during the training process.|
|**Gradient descent Algorithm**|Updates the weights (θ) by subtracting the gradient of the cost function with respect to the weights, scaled by a learning rate, to iteratively minimize prediction errors and improve the model.|





