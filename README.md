# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the NumPy library
2. Get the coefficient matrix and constant matrix from the user.
3. Apply Gaussian Elimination method to reduce the matrix into row echelon form and find the solution.
4. Display the values of the unknown variables as the output.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Varuna R
RegisterNumber: 212225040483
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
n = int(input())

a = [[0 for _ in range(n + 1)] for _ in range(n)]

for i in range(n):
    for j in range(n + 1):
        a[i][j] = float(input())


for k in range(n - 1):
    for i in range(k + 1, n):
        factor = a[i][k] / a[k][k]
        for j in range(k, n + 1):
            a[i][j] -= factor * a[k][j]


x = [0 for _ in range(n)]

for i in range(n - 1, -1, -1):
    x[i] = a[i][n]
    for j in range(i + 1, n):
        x[i] -= a[i][j] * x[j]
    x[i] /= a[i][i]

for i in range(n):
    print(f"X{i} = {x[i]:.2f}", end=" ")
*/
```

## Output:
![gaussian elimination]()
<img width="1256" height="599" alt="image" src="https://github.com/user-attachments/assets/0705b1fd-745e-4969-9af7-00c3fe5f6acd" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

