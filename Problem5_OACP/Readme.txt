1. Main Loop:
    -Continuously reads input for n.
    -Creates an array a of size n and reads n integers into it.
    -Reads input for m.
    -Creates an array b of size m and reads m integers into it.
    -Initializes a map mp to store the frequency of integers in array b.
    -Initializes cnt to 0 to count the number of pairs.
    -Sorts arrays a and b.
2. Pair Counting:
    -Iterates through each element of array a and b.
    -For each element a[i] in a, and each element b[j] in b:
      -If the frequency of b[j] in mp is less than 1, continue to the next iteration.
      -If the absolute difference between a[i] and b[j] is less than or equal to 1:
        -Increment cnt.
        -Decrement the frequency of b[j] in mp.
        -Break out of the inner loop.
3. Output:
    -Prints the value of cnt modulo MOD.