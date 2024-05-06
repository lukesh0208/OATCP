1. Include necessary libraries: <iostream> for input/output operations and <vector> for using vectors.
2. Define a constant MOD which is set to 10^9 + 7.
3. Define the main() function:
a. Disable the synchronization between C and C++ standard streams and untie the cin and cout streams for faster I/O.
b. Declare a variable n to store the size of the grid.
c. Read the size of the grid from the input.
4. Create a 2D vector dp of size (n+1) x (n+1) initialized with zeros. This vector will store the number of ways to reach each cell in the grid.
5. Set the base case dp[0][0] = 1, as there is only one way to reach the starting cell.
6. Iterate through each row of the grid:
a. Read a string s representing the obstacles in the current row.
b. Iterate through each column of the grid:
    -If the current cell is not an obstacle ('*'):
      -If the current row is greater than 0, add the number of ways to reach the current cell from the cell above it (dp[i][j] += dp[i - 1]      [j]).
      -If the current column is greater than 0, add the number of ways to reach the current cell from the cell to its left (dp[i][j] +=   dp[i][j - 1]).
      -Modulo the result with MOD.
    -If the current cell is an obstacle, set dp[i][j] = 0.
7. Output the number of ways to reach the bottom-right corner of the grid (dp[n - 1][n - 1]), modulo MOD. If n is 0, output -1.
8. Return 0 to indicate successful execution.