<b>Bubble Sort</b>

Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in wrong order.

Example:<br>
First Pass:<br>
( 5 1 4 2 8 ) –> ( 1 5 4 2 8 ), Here, algorithm compares the first two elements, and swaps since 5 > 1.<br>
( 1 5 4 2 8 ) –>  ( 1 4 5 2 8 ), Swap since 5 > 4<br>
( 1 4 5 2 8 ) –>  ( 1 4 2 5 8 ), Swap since 5 > 2<br>
( 1 4 2 5 8 ) –> ( 1 4 2 5 8 ), Now, since these elements are already in order (8 > 5), algorithm does not swap them.<br>

Second Pass:<br>
( 1 4 2 5 8 ) –> ( 1 4 2 5 8 )<br>
( 1 4 2 5 8 ) –> ( 1 2 4 5 8 ), Swap since 4 > 2<br>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 )<br>
( 1 2 4 5 8 ) –>  ( 1 2 4 5 8 )<br>
Now, the array is already sorted, but our algorithm does not know if it is completed. The algorithm needs one whole pass without any swap to know it is sorted.<br>

Third Pass:<br>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 )<br>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 )<br>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 )<br>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 )<br>

<b>Optimized Implementation:</b><br>
The above function always runs O(n^2) time even if the array is sorted. It can be optimized by stopping the algorithm if inner loop didn’t cause any swap.<br>

<b>Worst and Average Case Time Complexity:</b> O(n*n). Worst case occurs when array is reverse sorted.<br>

<b>Best Case Time Complexity:</b> O(n). Best case occurs when array is already sorted.<br>

<b>Auxiliary Space:</b> O(1)<br>

</b>Boundary Cases:</b> Bubble sort takes minimum time (Order of n) when elements are already sorted.<br>

<b>Sorting In Place:</b> Yes<br>

<b>Stable:</b> Yes<br>

Due to its simplicity, bubble sort is often used to introduce the concept of a sorting algorithm.<br>
In computer graphics it is popular for its capability to detect a very small error (like swap of just two elements) in almost-sorted arrays and fix it with just linear complexity (2n). For example, it is used in a polygon filling algorithm, where bounding lines are sorted by their x coordinate at a specific scan line (a line parallel to x axis) and with incrementing y their order changes (two elements are swapped) only at intersections of two lines.<br>
