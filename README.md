<H1 align="center">Multi Linear Regression From Scratch</H1>

In this repository we will be creating Multi Linear Regression Model from scratch using Numpy. We are going to use Iris dataset for this problem. 

# Steps for creating training the model:
1.  We build our hypothesis.
2.  Randomly initialize parameters.
3.  Create Loss function
4.  Find local derivative of loss function.
5.  Apply gradient descent to update the weights.
6.  Repeat 4 and 5 step unless epochs are finished or our loss is close to zero.

# Pre-processing the dataset:
    As we are going to use only numpy, so, we have to convert the data X, Y to arrays. I also inserted a column in X of ones because as we know that we have theta zero in the hypothesis so we have to insert one column so that we can multiply it with vector of theta.
    We are also going to randomly intialize value for theta's.

# Necessary Functions for Linear Regression
1. hypothesis()
2. cost_function()
3. der_cost_function()
4. gradient_descent_function()
5. train_function(no_of_it_train,no_of_it_print_cost,lr=0.0001)
6. Predict(X)
7. get_weights()
8. printer()

# 1. hypothesis():
    This function is calculating hypothesis by taking dot product of X and theta vectors.
# 2. cost_function():
    This function is calculating cost by taking mean of (Y - hypothesis())**2.
# 3. der_cost_function():
    This function is calculating derivative of cost function by taking dot product of (Y - hypothesis()) and X. After that it take mean of this dot product and then multiply it with -2.
# 4. gradient_descent_function():
    This function is calculating gradient descent meaning new value for theta by first taking derivative of cost function and then use this formula: new_theta = old_theta - learning rate * derivative of cost function.
# 5. train_function(no_of_it_train,no_of_it_print_cost,lr=0.0001):
    This function is used to train our regression model for no_of_it_train and print cost after no_of_it_print_cost. 
# 6.  Predict(X):
    This function is used to predict value on given X and returns it. 
# 7. get_weights():
    This function is used to return value of theta's.
# 8. printer():
    This function is used to print value of X, Y, theta's.


# Happy Coding:)
