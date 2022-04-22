# Quick Sort Algorithm



##  Pseudo Code
low  --> Starting index,  high  --> Ending index   <br/>
quickSort(arr[], low, high)                         <br/>
{                                                   <br/>
&emsp;    if (low < high)                                 <br/>
&emsp;    {                                                 <br/>
&emsp;&emsp;        /* pi is partitioning index, arr[pi] is now   <br/>
&emsp;&emsp;           at right place */                            <br/>
&emsp;&emsp;        pi = partition(arr, low, high);                   <br/>
                                                        <br/>
&emsp;&emsp;        quickSort(arr, low, pi - 1);  // Before pi    <br/>
&emsp;&emsp;        quickSort(arr, pi + 1, high); // After pi     <br/>
&emsp;    }                   <br/>
}     <br/>

## Time Complexity
Best Case: O(nlog2n) => 2 in base (the arrayy is unsorted and pivot is in the middle.) <br/>
Worst Case: O(n^2) (the array is already sorted and pivot is in the first index.) <br/>
Average Case: O(nLog2n) =>2 in base <br/>

##  Workflow
[40][20][10][80][60][50][7][30][100]<br/>
40 is pivot <br/>
20 is top index <br/>
100 is bottom index <br/>

1.  while data[top_index] <= data[pivot]     <br/>
&emsp;&emsp;  ++top_index           <br/>
2.  while data[bottom_index]>data[pivot]    <br/>
&emsp;&emsp;  --bottom_index      <br/>
3.  if top_index<bottom_index     <br/>
&emsp;&emsp;  swap(data[top_index],data[bottom_index])    <br/>
4.  while bottom_index>top_index          <br/>
&emsp;&emsp;  go to 1                       <br/>
5.  swap(data[top_index],data[pivot_index])         <br/>








