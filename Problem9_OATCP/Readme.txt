1.Read the integer m representing the size of the array.
2.Read the array arr of size m.
3.Read the integer n.
4.Initialize variables i to track the index of the array, ans to count the number of steps, and cnt to track the current value.
5.Iterate until cnt reaches or exceeds n:
      Check if i is within bounds (i < m) and if the current element arr[i] is less than or equal to cnt.
         If true, increment cnt by arr[i] and increment i.   
         If false, double the value of cnt and increment ans.
6.Output the value of ans representing the minimum number of steps required to reach or exceed n.