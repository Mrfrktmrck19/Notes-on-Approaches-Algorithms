 #  Bubble Sort
##  How does The Bubble Sort work?
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in the wrong order. <br/>
Example:  <br/>
First Pass: <br/>
( 5 1 4 2 8 ) –> ( 1 5 4 2 8 ), Here, algorithm compares the first two elements, and swaps since 5 > 1. <br/>
( 1 5 4 2 8 ) –>  ( 1 4 5 2 8 ), Swap since 5 > 4 <br/>
( 1 4 5 2 8 ) –>  ( 1 4 2 5 8 ), Swap since 5 > 2 <br/>
( 1 4 2 5 8 ) –> ( 1 4 2 5 8 ), Now, since these elements are already in order (8 > 5), algorithm does not swap them. <br/>
Second Pass: <br/>
( 1 4 2 5 8 ) –> ( 1 4 2 5 8 ) <br/>
( 1 4 2 5 8 ) –> ( 1 2 4 5 8 ), Swap since 4 > 2 <br/>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 ) <br/>
( 1 2 4 5 8 ) –>  ( 1 2 4 5 8 ) <br/>
Now, the array is already sorted, but our algorithm does not know if it is completed. The algorithm needs one whole pass without any swap to know it is sorted. <br/>
Third Pass:  <br/>
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 ) 
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 ) 
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 ) 
( 1 2 4 5 8 ) –> ( 1 2 4 5 8 ) 
### Pseudo Code
for i =1 to length[A] <br/>
&ensp;  for j = 1 to length[A-1-i] <br/>
&ensp;&ensp;    if A[j]>A[j++] <br/>
&ensp;&ensp;&ensp;      exchange(A[j],A[j++]) <br/>
##  Space Complexity
The space complexity for Bubble Sort is O(1), because only a single additional memory space is required i.e. for temp variable.
##  Time Complexity
The always runs O(n^2) time even if the array is sorted. It can be optimized by stopping the algorithm if the inner loop didn’t cause any swap. 

![](https://github.com/Mrfrktmrck19/Notes-on-Approaches-Algorithms/blob/main/images/bubblesort1.jpeg)
