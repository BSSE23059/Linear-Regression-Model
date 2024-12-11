# Linear-Regression-Model
Build the Linear Regression class like that of Scikit Learn LinearRegression class.

This project implements a simple Linear Regression model in Python from scratch. The class includes methods to train the model (`fit`) and make predictions (`predict`).

---

## Derivation of the Equation

In Python, this is implemented as:
```python
num = 0
den = 0
for i in range(x_train.shape[0]):
    num = num + ((x_train[i] - x_train.mean()) * (y_train[i] - y_train.mean()))
    den = den + ((x_train[i] - x_train.mean()) * (x_train[i] - x_train.mean()))
m = num / den
