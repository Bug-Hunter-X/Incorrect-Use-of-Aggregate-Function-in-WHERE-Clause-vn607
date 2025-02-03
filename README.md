# Incorrect Use of Aggregate Function in WHERE Clause
This SQL query attempts to find employees in the Sales department whose salary is greater than the average salary across all employees. However, it contains a common error: using an aggregate function like AVG() directly within the WHERE clause.  Aggregate functions operate on sets of rows, and the WHERE clause filters individual rows before aggregation occurs. This leads to an incorrect result.

The provided `bug.sql` demonstrates the erroneous query, while `bugSolution.sql` offers a corrected approach.