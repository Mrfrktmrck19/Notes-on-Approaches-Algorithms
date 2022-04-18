# Seelction Sort

##  How does The Selection Algorithm work?
The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning.<br/>
The algorithm maintains two subarrays in a given array.<br/>
1) The subarray which is already sorted. <br/>
2) Remaining subarray which is unsorted.<br/>
In every iteration of selection sort, the minimum element (considering ascending order) from the unsorted subarray is picked and moved to the sorted subarray. <br/>
![](https://github.com/Mrfrktmrck19/Notes-on-Approaches-Algorithms/blob/main/images/selectionsortalgo.jpeg)

## Time & Space Complexity
Time Complexity Θ(n^2)
Space Complexity O(1)

##  Pseudo Code
&ensp; for i=0 to n-1          <br/>
&ensp;&ensp;  key=i                 <br/>
&ensp;&ensp;  for j=i+1 to n        <br/>
&ensp;&ensp;&ensp;    if(A[j]>A[key])     <br/>
&ensp;&ensp;&ensp;&ensp;      key=i             <br/>
&ensp;&ensp;  swapping(A[i],A[key]) <br/>
