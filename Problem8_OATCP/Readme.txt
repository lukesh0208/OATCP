1.Read the input string num and integer k.
2.Initialize an empty string ans to store the resulting number.
3. Iterate through each digit c in the input string num:
    3.1. While ans is not empty, the last digit in ans is greater than c, and k is still greater than 0, remove the last digit from ans and        decrement k.
    3.2. Append the current digit c to ans if ans is not empty or if c is not '0'.
4.After iterating through all digits, if k is still greater than 0, remove digits from the end of ans until k becomes 0.
5.If ans is empty at this point, assign it the value '0'.
6.Output the resulting string ans.