1. maxRotateValue function:
    -Accepts a reference to a vector of integers nums.
    -Initialize n as the size of the vector nums.
    -If n is 0, return 0.
    -Initialize a vector dp of size n + 1.
    -Initialize total_sum and current_sum to 0.
    -Iterate through the elements of nums:
      -Update total_sum by adding the current element.
      -Update current_sum by adding the product of the index and the current element.
    -Set dp[0] to current_sum.
    -Iterate from 1 to n - 1:
      -Update dp[i] using the formula: dp[i] = dp[i - 1] + total_sum - n * nums[n - i].
    -Find the maximum value in the vector dp.
    -Return the maximum value.
2. main function:
    -Accepts input for the number of elements n.
    -Accepts input for the elements of the vector nums.
    -Calls the maxRotateValue function with the vector nums.
    -Prints the maximum rotate value returned by the function.