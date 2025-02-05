# Linear Regression Implementation

## Overview
This project demonstrates the implementation of Linear Regression from scratch using Python and NumPy. The model is trained on a synthetic dataset generated using Scikit-learn and evaluated for performance.

## Dataset
A random dataset is generated using `datasets.make_regression()` with the following parameters:
- **Number of Samples:** 100
- **Number of Features:** 1 (Simple Linear Regression)
- **Noise:** 20 (to introduce variability in the data)
- **Random State:** 4 (for reproducibility)

## Steps in the Implementation

### 1. Loading the Dataset
The dataset is generated using the Scikit-learn `datasets.make_regression()` function, creating an independent variable `X` and a dependent variable `y`.

### 2. Splitting the Data
The dataset is divided into training (80%) and testing (20%) subsets using `train_test_split()`.

### 3. Training the Linear Regression Model
The model is implemented in a separate Python script (`linear_regression.py`) and follows these steps:
- Initializes the weights and bias to zero.
- Uses gradient descent to update weights iteratively.
- Minimizes the Mean Squared Error (MSE) as the cost function.

### 4. Making Predictions
For a given test sample, the predicted values are computed using:
\[ y_{predicted} = X \cdot w + b \]
where `w` represents weights and `b` represents bias.

### 5. Evaluating the Model
The predictions are compared with the actual labels, and the Mean Squared Error (MSE) is computed using:
\[ MSE = \frac{1}{n} \sum (y - y_{predicted})^2 \]

### 6. Results and Visualization
- A scatter plot of the dataset is generated to visualize the data distribution.
- The best-fit regression line is plotted to show how well the model fits the data.

## Accuracy Measure
The Mean Squared Error (MSE) is used as the primary metric to evaluate model performance. A lower MSE indicates better model performance.

## Dependencies
- NumPy
- Matplotlib
- Scikit-learn

## Conclusion
This implementation demonstrates a simple but effective approach to understanding the workings of Linear Regression using Python. The model can be extended to multiple features for a more complex analysis.

