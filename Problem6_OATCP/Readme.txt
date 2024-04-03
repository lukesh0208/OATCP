1.Input the number of items n, costs of the items, and the number of coins available.
2.Store the costs of items in a vector costs.
3.Sort the costs vector in non-decreasing order.
4.Initialize a variable ans to count the number of items bought.
5.Iterate through the sorted costs vector:
  5.1 If the number of coins is sufficient to buy the current item, decrement the coins by the cost of the item and increment ans.
  5.2 If not, break out of the loop.
6.Output the value of ans, representing the maximum number of items bought with the given number of coins.