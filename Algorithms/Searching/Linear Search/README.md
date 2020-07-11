A simple approach is to do linear search, i.e

Start from the leftmost element of arr[] and one by one compare x with each element of arr[].

If x matches with an element, return the index.

If x doesn’t match with any of elements, return -1.

![](Linear-Search.png)  

Efficiency:
In general, for a list of length N, the worst case is N comparisons and the average case is N/2 comparisons.
