# Gradient Descent Optimization

This Python script implements the gradient descent optimization algorithm to find the optimal values for a given mathematical function. The user is prompted to enter an expression, learning rate, number of iterations, and starting points for `x` and `y`. The script then performs gradient descent to find the optimal values of `x` and `y` that minimize the given function.

## Prerequisites

Make sure you have the following libraries installed:

- `numpy`
- `math`
- `sympy`
- `numdifftools`

You can install them using:

```bash
pip install numpy math sympy numdifftools
```

## Usage

1. Run the script: `python gradient_descent.py`
2. Enter the expression to be minimized.
3. Input the learning rate, number of iterations, and starting points for `x` and `y` when prompted.

## Functions

### `gradient(fcn, var, var_x, var_y)`

Calculates the gradient of the given function with respect to the specified variable at the provided `var_x` and `var_y` values.

### `function_value(fcn, varx, vary)`

Calculates the value of the given function at the provided `varx` and `vary` values.

### `gradient_descent(function, learning_rate, iteration, x_start, y_start)`

Performs gradient descent optimization on the given function with the specified learning rate, number of iterations, and starting points for `x` and `y`.

## Example

```python
input_expr = input('Enter an expression: ')
learningRate = float(input('Enter the learning rate: '))
Iteration = int(input('Enter number of iteration: '))
X_Start = int(input('Enter starting point of x: '))
Y_Start = int(input('Enter starting point of y: '))

value = gradient_descent(input_expr, learningRate, Iteration, X_Start, Y_Start)
print(value)
```

## Note

- Ensure the entered expression is a valid mathematical expression that can be processed by the `sympy` library.
- Adjust the learning rate and number of iterations based on the specific optimization problem and convergence behavior.

---
