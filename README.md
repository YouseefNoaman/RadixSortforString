# RadixSortforString
A begginer's guide to radix sort for String input

This is ONE of a series made to be helpful to newbs in the Data struuctures and algorithms, to help them grasp the algorithms and its intuitions, i hope you find it helpful, if you want any more clarification or an algorithm to be broken down by me in this style just send a mail, thanks a lot for checking this.

this algorithm makes certain assumptions about the data:

    1)the data MUST have the same width and radix
  
    2)the data must be integers or strings
  
- width: means how many digits are in the data element, "hello" width = 5, 824 width = 3

- radix: it means the counting system, binary system(0, 1) has radix = 2, decimal system(0 .. 9) has radix = 10

- this sort algorithm needs to use a stable sort algorithm at each step, usually it is the stable version of counting sort

- O(n) generally, but often slower than O(n log n), because of the overhead of separating values at each step

- it is a stable algorithm

- in-place algorithm in this implementation, other stable sorting algorithms if used, it may not be an in-place algorithm.

- it sorts from the least significant digit to the most significant digit, right to left, like 824, sorted firstly 4 then 2 lastly 8, or if it is used to sort strings, "hello" would be sorted by 'o' then 'l', 'l', 'e', and lastly 'h'.
