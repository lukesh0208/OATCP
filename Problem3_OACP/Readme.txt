1. Include necessary libraries and define macros for convenience.
2. Define n to store the size of the vector.
3. Define mod as 10^9 + 7.
4. Main function:
    -Disable synchronization between C and C++ standard streams and untie the cin and cout streams for faster I/O.
    -Read input n.
    -Create a vector nums to store n integers.
    -Read n integers into the vector.
5. Initialize maxi to INT_MIN and prd to 1.
6. Iterate through the vector nums:
    -Update prd by taking the product of prd with the current element modulo mod.
    -Update maxi to the maximum of maxi and prd.
7. Output the maximum product maxi.