# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy and Use lu(),lu_solve(),lu_factor() to get the solutions
4. End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by:R S Sashwath
RegisterNumber: 26003043
'''
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
'''Program to solve a matrix using LU decomposition.
Developed by: R S Sashwath
RegisterNumber: 26003043
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:
1.
<img width="1185" height="392" alt="image" src="https://github.com/user-attachments/assets/a106b5f6-ee2a-4100-98ab-34a593a0aae8" />

2.
<img width="1237" height="238" alt="image" src="https://github.com/user-attachments/assets/96a243e7-2f00-48d3-939f-7be78e445833" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

