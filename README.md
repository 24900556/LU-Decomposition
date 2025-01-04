# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the necessary libraries.
2. Input a square matrix 𝐴
3. Use the lu() function from the scipy.linalg module to compute:
    
    P: Permutation matrix

    L: Lower triangular matrix
    
    U: Upper triangular matrix
4. Display the matrices L and 𝑈

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by:R.R.Madhumitha
RegisterNumber: 24900556
*/
```
    import numpy as np
    from scipy.linalg import lu
    A=np.array(eval(input()))
    P,L,U=lu(A)
    print(L)
    print(U)
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by:R.R.Madhumitha 
RegisterNumber: 24900556
*/
```
    import numpy as np
    from scipy.linalg import lu_factor,lu_solve
    A=np.array(eval(input()))
    B=np.array(eval(input()))
    lu,piv=lu_factor(A)
    X=lu_solve((lu,piv),B)
    print(X)

## Output:
![i](<Screenshot 2024-12-06 053123.png>)
![ii](<Screenshot 2024-12-06 053145.png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

