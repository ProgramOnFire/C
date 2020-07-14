<b>Insertion Sort</b><br>

Insertion sort is a simple sorting algorithm that works the way we sort playing cards in our hands.<br>

<b>Algorithm</b><br>
// Sort an arr[] of size n<br>
insertionSort(arr, n)<br>
Loop from i = 1 to n-1.<br>
……a) Pick element arr[i] and insert it into sorted sequence arr[0…i-1]<br>

<b>Example:</b><br>
<img src="insertionsort.png"><br><br>

<b>Time Complexity:</b> O(n*2)<br>

<b>Auxiliary Space:</b> O(1)<br>

<b>Boundary Cases:</b> Insertion sort takes maximum time to sort if elements are sorted in reverse order. And it takes minimum time (Order of n) when elements are already sorted.<br>

<b>Algorithmic Paradigm:</b> Incremental Approach<br>

<b>Sorting In Place:</b> Yes<br>

<b>Stable:</b> Yes<br>

<b>Online:</b> Yes<br>

<b>Uses:</b> Insertion sort is used when number of elements is small. It can also be useful when input array is almost sorted, only few elements are misplaced in complete big array.<br>
