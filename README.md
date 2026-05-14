# MAI---EX-5
# LU Decomposition 
## Name: NISHMA SHERIN . K 
## Register Number: 212224240104

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## Step 1:
Import required libraries (NumPy and SciPy) and read the input matrix A.

## Step 2:
Perform LU decomposition of matrix A and obtain L and U matrices.

## Step 3:
Display the L and U matrices to verify the decomposition.

## Step 4:
If required, read matrix/vector B and solve the system AX = B using LU factorization.

## Program:
(i) To find the L and U matrix
```
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot= lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:


<img width="1242" height="491" alt="Screenshot 2026-05-14 091139" src="https://github.com/user-attachments/assets/075645d3-cc13-4d7b-a566-da6ca9a48f6a" />

<img width="1240" height="366" alt="Screenshot 2026-05-14 091157" src="https://github.com/user-attachments/assets/8bbe2da8-ca3e-413a-83f1-e4835bf5e360" />







## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
