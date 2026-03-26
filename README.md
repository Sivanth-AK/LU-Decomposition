# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Import the numpy module to use built-in functions for calculations. 
Step 2: Import the lu function from scipy.linalg to perform LU decomposition. 
Step 3: Read the input matrix, perform LU decomposition using lu(A), and print the L matrix and U matrix. 
Step 4: End the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: SIVANTH T
RegisterNumber: 212225240150
*/
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
p,l,u=lu(matrix)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: SIVANTH T
RegisterNumber: 212225240150
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input())) 
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:
![lu decomposition]()
i) <img width="1106" height="383" alt="image" src="https://github.com/user-attachments/assets/4e6a3023-cbf2-4d1d-8293-383fb79614a7" />

ii)<img width="765" height="165" alt="image" src="https://github.com/user-attachments/assets/0758771a-20c4-4d42-9dea-0eaa53a31883" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

