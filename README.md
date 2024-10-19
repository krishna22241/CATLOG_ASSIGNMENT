# CATLOG_ASSIGNMENT
1. Read the JSON input from the file.
2. For each entry (x, y), decode the y value using its base.
3. Form the augmented matrix for the system of linear equations:
   A = [x^m, x^(m-1), ..., x^1, 1] for each point.
   Y = [y1, y2, ..., yk] (decoded y values)
4. Perform Gaussian elimination on the augmented matrix to convert it into an upper triangular matrix.
5. Use back substitution to solve for the coefficients [a_m, a_(m-1), ..., a_1, c].
6. Print the constant term `c` (this is the secret).
