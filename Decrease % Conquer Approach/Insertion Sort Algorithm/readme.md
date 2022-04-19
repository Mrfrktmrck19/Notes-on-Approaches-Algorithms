# Insertion Sort Algorithm

This algorithm has best case and worst case. Best case is the array already sorted array. Worst case is reverse sorted array (exp. descending array but we want ascending).

##  How does The Insertion Algorithm work
Insertion sort is a simple sorting algorithm that works similar to the way you sort playing cards in your hands. The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part. <br/>
Algorithm : <br/>
To sort an array of size n in ascending order:  <br/>
1: Iterate from arr[1] to arr[n] over the array. <br/>
2: Compare the current element (key) to its predecessor. <br/>
3: If the key element is smaller than its predecessor, compare it to the elements before. Move the greater elements one position up to make space for the swapped element.  <br/>
