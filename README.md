# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

### (i) To find the L and U matrix
1. Imports numpy and scipy.linalg.
2. Accepts a nested list (matrix) as input from the user.
3. Converts the input to a NumPy array.
4. Performs LU decomposition using scipy.linalg.lu.
5. Stores and prints the L (I_matrix) and U (u_matrix) matrices.

### (ii) To find the LU Decomposition of a matrix
1. Import numpy for array handling and lu_factor, lu_solve from scipy.linalg.
2. Input Matrix from User and Convert the input into a NumPy array (mat).
3. Prompt the user to enter the constant vector and Convert it into a NumPy array( l ).
4. Apply the lu_factor() function to the matrix (mat) and store it (x).
5. Use lu_solve() with the LU decomposition (x) and the constant vector( l ).
6. Print the result.
   
## Program:
(i) To find the L and U matrix
```python
'''
Developed by: Arunsamy D
RegisterNumber: 212224240016
'''
import numpy as np
from scipy.linalg import lu

mat = eval(input())
p , l, u = lu(mat)
print(l)
print(u)
```

(ii) To find the LU Decomposition of a matrix
```python
'''
Developed by: Arunsamy D
RegisterNumber: 212224240016
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
mat=np.array(eval(input()))
l=np.array(eval(input()))
x=lu_factor(mat)
sln = lu_solve(x, l)
print(sln)
```

## Output:

![Screenshot 2025-05-21 072356](https://github.com/user-attachments/assets/70e12de8-3e03-47c5-aef8-8b96eecd9165)

![Screenshot 2025-05-21 072429](https://github.com/user-attachments/assets/2b55f7eb-6fe2-4305-9b42-943e088e42cc)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

