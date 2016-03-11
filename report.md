UECM3033 Assignment #2 Report
========================================================

- Prepared by: Liew Kok Hoong
- Tutorial Group: T3

--------------------------------------------------------

## Task 1 --  $LU$ Factorization or SOR method

The reports, codes and supporting documents are to be uploaded to Github at: 

[https://github.com/1203222/UECM3033_assign2](https://github.com/your_github_id/UECM3033_assign1)

Explain your selection criteria here.

SOR method is preferred method for solving linear system if a matrix A be a positive definite matrix which mean all the eigenvalues of matrix A are positive( all eigenvalues of matrix A > 0 ). The formula of optimal ω for the SOR method is calculated if and only if matirx A  be a positive definite matrix. Besides, the range of the ω is between 0 and 2. 

LU factorisation is preferred method for solving linear system if a matrix A is not a positive definite matrix. Moreover, the LU factorisation will be preferred if solve Ax=b for different values of b, as one only need to factorise A once and the same L and U can be applied to the different values of b repeatly. This is because the matrix A will be factorised into two triangular form LU and solve the Ax=b by substitution.

Explain how you implement your `task1.py` here.

The first linear system is 

\begin{align} 2 x_1 + 1 x_2 + 6 x_3 &= 9,\\ 8 x_1 + 3 x_2 + 2 x_3 &= 13,\\ 1 x_1 + 5 x_2 + 1 x_3 &= 7. \end{align}

\begin{align} Solution = [ x_1 = 1, x_2 = 1, x_3 = 1 ] \end{align}

The second linear system is 

\begin{align} 6566 x_1 - 5202 x_2 - 4040 x_3 - 5224 x_4 + 1420 x_5 + 6229 x_6 &= 17603,\\ 4104 x_1 + 7449 x_2 - 2518 x_3 - 4588 x_4 - 8841 x_5 + 4040 x_6 &= -63286,\\ 5266 x_1 - 4008 x_2 + 6803 x_3 - 4702 x_4 + 1240 x_5 + 5060 x_6 &= 56563,\\ -9306 x_1 + 7213 x_2 + 5723 x_3 + 7961 x_4 - 1981 x_5 - 8834 x_6 &= -26523.5,\\ -3782 x_1 + 3840 x_2 + 2464 x_3 - 8389 x_4 + 9781 x_5 - 3334 x_6 &= 103396.5,\\ -6903 x_1 + 5610 x_2 + 4306 x_3 + 5548 x_4 - 1380 x_5 + 3539 x_6 &= -27906. \end{align}

\begin{align} Solution = [ x_1 = -19.26962981, x_2 = -16.65580305, x_3 = 4.9615347, x_4 = -18.58795701, x_5 = -9.30020118, x_6 = -1.02242731 ] \end{align}

I checked the answers for the two linear system by substituted back all the x values into the linear equations.

Firstly, I will write the python code for LU factorisation and SOR method in order to solve the two linear systems. Next, I put the condition which is all the eigenvalues of matrix A are positive( all eigenvalues of matrix A > 0 ) to check whether matrix A is positive definite matrix or not. If matrix A is positive definite matrix, SOR method will be selected and applied to solve the two linear systems. Otherwise, the two linear systems will be solve by using LU factorisation. Finally, the answers of two linear systems will be printed out and stated 'Solve by sor(A,b)' or 'Solve by lu(A,b)'.  



---------------------------------------------------------

## Task 2 -- SVD method and image compression

Put here your picture file 

!['Metalslug.jpg'](Lenna.png)

How many non zero element in $\Sigma$?

Answer: 11

Put here your lower and better resolution pictures. Explain how you generate
these pictures from `task2.py`.

What is a sparse matrix?

Sparse matrix is a matrix in which most of the elements are zero.



-----------------------------------

<sup>last modified: 11/3/2016</sup>
