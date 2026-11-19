# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1: Import the required Python libraries (NumPy, Pandas, Matplotlib, Scikit-learn) and load the Salary dataset.

2: Separate the dataset into independent variable (Years of Experience) and dependent variable (Salary) and train the Decision Tree Regressor model using the training data.

3: Accept Years of Experience as input from the user.

4: Use the trained model to predict and display the salary corresponding to the given experience

## Program:
```PYTHON
/*

Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: JOANNE JAISON
RegisterNumber:  212225020017

# Import libraries
import numpy as np
import pandas as pd
from sklearn.tree import DecisionTreeRegressor

# Load dataset
dataset = pd.read_csv("C:/Users/acer/Downloads/Salary.csv")

# Select numeric column (Level / Experience)
X = dataset.iloc[:, 1:2].values   # only Level column
y = dataset.iloc[:, 2].values     # Salary column

# Create model
model = DecisionTreeRegressor(random_state=0)

# Train the model
model.fit(X, y)

# Get input from user
exp = float(input("Enter Level / Years of Experience: "))

# Predict salary
predicted_salary = model.predict([[exp]])

# Display output
print("Predicted Salary:", predicted_salary[0])
 
*/
```

## Output:
<img width="778" height="76" alt="Screenshot 2026-11-19 160308" src="https://github.com/user-attachments/assets/c222e2a4-b88f-4241-ae43-59c23d1868fe" />



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
