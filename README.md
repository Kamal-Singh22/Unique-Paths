# Unique-Paths
A robot is located at the top-left corner of a grid (m x n). The robot can only move either down or right at any point in time. The robot is trying to reach the bottom-right corner of the grid (m x n).
Explanation:
Dynamic Programming Table:

dp[i][j] represents the number of unique paths to cell (i, j).
The value is calculated as dp[i-1][j] + dp[i][j-1], which means:
Paths coming from the cell above (dp[i-1][j]).
Paths coming from the cell to the left (dp[i][j-1]).
Initialization:

The first row and first column are initialized to 1 because there is only one way to traverse those (either keep going right or down).
Output:

The result is stored in dp[m-1][n-1], representing the bottom-right corner of the grid.
