# Linear Regression
## 1) Generating the Dataset
A synthetic dataset is created using make_regression() from sklearn.datasets, with:

n_samples=100: 100 random samples
n_features=1: A single feature for simple linear regression
noise=20: Adds some randomness to the data
random_state=4: Ensures reproducibility
The dataset consists of one input feature and one output variable.

## 2) Splitting the Data
The dataset is divided into training (80%) and testing (20%) subsets using train_test_split().

## 3) Training the Linear Regression Model
The Linear_regression class is implemented to learn a linear relationship between X and y.
The model is trained using gradient descent to optimize weights (w) and bias (b).
The loss function used is Mean Squared Error (MSE), and gradients are computed to update the parameters.
## 4) Making Predictions
The learned weights and bias are used to compute y_predicted = wX + b for the test set.
## 5) Evaluating the Model
The model's performance is measured using Mean Squared Error (MSE):
 
## 6) Results and Visualization
The dataset is visualized using scatter plots to show data distribution.
A regression line is plotted to show how well the model fits the data.
