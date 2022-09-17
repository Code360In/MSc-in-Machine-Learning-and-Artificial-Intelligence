# Matrix Operations - II

Let's now study two commonly used matrix operations - **transpose** and **inverse.**

## Transposing a Matrix

The **transpose** of a matrix produces a matrix in which the rows and columns are interchanged. For example, the transpose of the matrix $A=\begin{bmatrix}7&0\\2&3\\-1&4\end{bmatrix}$ is $A^T=\begin{bmatrix}7&2&-1\\0&3&4\end{bmatrix}$

Note that the size of the transpose matrix can different from the original matrix, as shown in this example.

In general, the transpose of a matrix satisfies the following:

- The transpose of an (m, n) matrix is a matrix of size (n, m)
- The value present at the index (i, j) in the original matrix will be present at the index (j, i ) in the transpose matrix

In Numpy, you can compute the transpose of a matrix A using A.T as follows:

```python
import numpy as np
A = np.array([[1, 3], 
             [2, 0]])
# transpose
print(A.T)
```

#### Transpose of a Matrix

Consider the following matrix 
$$\large{X=\begin{bmatrix}4&2&5\\3&2&8\\5&2&9\\7&2&1\end{bmatrix}}$$
Qn: Now, consider the matrix U=(X′*X), where X' is the transpose of X. Which of the following dimensions can a matrix A have, if U*A is known to exist?
- 3x3

- 5x3

- 5x5

- 3x5

Ans: A & D. *Since X' is a 3 x 4 matrix, U = X'X is a 3 x 3 matrix. For UA to exist, then the number of rows in A should be equal to 3.*

## **Matrix Inverse**

The inverse of a matrix A is a matrix A−1 such that their product AA−1=I , i.e. the identity matrix. You can study the basics of matrix inverse in [the following Khan Academy video](https://www.youtube.com/watch?v=iUQR0enP7RQ), though you will not need to compute the inverses of matrices manually in this program - you can skip the video if you are familiar with the basic idea.

However, it is useful to know how to compute the inverse in Numpy. You can do that using the method np.linalg.inv(A) as shown below. Also, note that matrices in Numpy can be created using either np.matrix() or using np.array().

```python
# inverse
A = np.array([[2, 1, -1], 
              [1, 0, -1], 
              [-2, 0, 1]])

np.linalg.inv(A)
```
