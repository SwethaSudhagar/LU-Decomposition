# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 5A)
1. start the program.
2. import the Numpy library and the lu function from scipy.linalg. 
3. get the input matrix from the user.
4. perform LU decomposition to find the lower triangular matrix(L) and upper triangular matrix(U).
5. Display the L and U matrices.
6. stop the program.

### 5B)
1. start the program.
2. import the Numpy library and the lu_factor and lu_solve functions from scipy.linalg.
3. get the coefficient matrix A and the constant matrix b as input from the user.
4. perform LU factorization of matrix A using lu_factor().
5. solve the system of equations using lu_solve() to find the solution matrix X.
6. Display the solution matrix X.
7. stop the program.


## Program:
### 5A) To find the L and U matrix
'''python
'''Program to find L and U matrix using LU decomposition.'''
Developed by: swetha s
RegisterNumber: 26012309 

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
'''


### 5B) To print X matrix (solution to the equations)
'''python
'''Program to solve a matrix using LU decomposition.'''
Developed by: swetha s
RegisterNumber: 26012309


# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
'''

## Output:
### 5A) <img width="621" height="715" alt="image" src="https://github.com/user-attachments/assets/e4b4c350-88a8-49e6-9acb-7b3f492a0839" />
### 5B) <img width="622" height="545" alt="image" src="https://github.com/user-attachments/assets/708d058f-79aa-4d3e-82e9-b9ea1c72c809" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

