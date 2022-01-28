# Different Ways to Sort (CS)

|Name|what it is|
|---|---|
|Insertion sort |The array is split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part<br/><br/>When iterating through items, if any item is smaller than its predecor, move it back until it is bigger<br/><br/>Worst/avg case: $O(n^2)$<br/>Best case: $O(n)$<br/>Good for: small n, small arrays |
|Merge sort     |Split the list in half until there's only one item in each list, then merge and sort all the lists back together<br/><br/>Worst/avg/best case: $O(n\log n)$<br/>Drawbacks: more memory, not good for long lists<br/>Good for: sorting linked list |
|Quicksort      |After choosing a pivot (which item should be pivot depends on how sorted/unsorted the arary is), swap items from the left and right hand side until the pivot is at the right index. Then, quicksort the left and right portion of the right index pivot. Do this again and again until the whole array is sorted.<br/><br/>Best/avg case: $O(n\log n)$<br/>Worst case: $O(n^2)$<br/>Good for: already know the type of array and can choose pivot smartly, for arrays, minimal additional memory required, good for certain types of processors<br/>Drawback: worst case is slow |
|Shell sort     |A variation of Insertion Sort. With the gap to skip and swap chosen, we would go through the list comparing items $gap$ apart, and swapping back to the start until not bigger. Repeat with --gap until 0, and list would be sorted.<br/>Best case: $O(n)$<br/>Avg case: $O(n\log (n)^2$<br/>Wrose case: base on gap size<br/>Allow for swapping items far apart.|
|Heap sort      |Transform list to a binary tree and sorting the binary tree by going from top down.<br/><br/>Creating binary tree takes $O(n)$, heapify binary tree takes $O(\log n)$<br/>Time Complexity: $O(n\log n)$<br/> |
|Bubble sort    |Repeatedly going through the list and swapping adjacent items, and iterating through the list until all adjacent items are in order.<br/><br/>Best case: $O(n)$<br/>Worse/avg case: $O(n^n)$<br/>Good only because its simple and nothing else|
|Radix sort     | Sort by digit|
|Counting sort  | |