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



---------------------------------------------------------

## Task 2 -- SVD method and image compression

Put here your picture file (Lenna.png)

![Lenna.png](Lenna.png)

How many non zero element in $\Sigma$?

Put here your lower and better resolution pictures. Explain how you generate
these pictures from `task2.py`.

What is a sparse matrix?


-----------------------------------

<sup>last modified: change your date here</sup>
