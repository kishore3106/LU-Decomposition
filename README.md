# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module and lu module from scipy.linalg to use the built-in functions for calculation
2. Prepare the lists from each linear equations and assign in np.array()
3. Using the lu(), we get three results (first is P, second is L and third is U) of the given matrix.
4. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable.
5. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Kishore B
RegisterNumber: 24900596
*/

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
p,l,u=lu(A)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Kishore B
RegisterNumber: 24900596
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)

```

## Output:

![Screenshot 2024-12-02 191331](https://github.com/user-attachments/assets/48a7f0bb-8fc7-4b93-b840-0868cb0afc56)

![image](https://github.com/user-attachments/assets/0064909a-ac70-4ebc-887d-5e7924ef6667)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

