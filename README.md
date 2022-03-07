# Data-Structure-and-Algorithms-Insertion-Sort

This is an in-place comparison-based sorting algorithm. Here, a sub-list is maintained which is always sorted. For example, the lower part of an array is maintained to be sorted. An element which is to be 'insert'ed in this sorted sub-list, has to find its appropriate place and then it has to be inserted there. Hence the name, insertion sort.

The array is searched sequentially and unsorted items are moved and inserted into the sorted sub-list (in the same array). This algorithm is not suitable for large data sets as its average and worst case complexity are of Ο(n2), where n is the number of items.

## How Insertion Sort Works?

We take an unsorted array for our example.

![](./assests/picture1.png)

Insertion sort compares the first two elements.

![](./assests/picture2.png)

It finds that both 14 and 33 are already in ascending order. For now, 14 is in sorted sub-list.

![](./assests/picture3.png)

Insertion sort moves ahead and compares 33 with 27.

![](./assests/picture4.png)

And finds that 33 is not in the correct position.

![](./assests/picture5.png)

It swaps 33 with 27. It also checks with all the elements of sorted sub-list. Here we see that the sorted sub-list has only one element 14, and 27 is greater than 14. Hence, the sorted sub-list remains sorted after swapping.

![](./assests/picture6.png)

By now we have 14 and 27 in the sorted sub-list. Next, it compares 33 with 10.

![](./assests/picture7.png)

These values are not in a sorted order.

![](./assests/picture8.png)

So we swap them.

![](./assests/picture9.png)

However, swapping makes 27 and 10 unsorted.

![](./assests/picture10.png)

Hence, we swap them too.

![](./assests/picture11.png)

Again we find 14 and 10 in an unsorted order.

![](./assests/picture12.png)

We swap them again. By the end of third iteration, we have a sorted sub-list of 4 items.

![](./assests/picture13.png)

This process goes on until all the unsorted values are covered in a sorted sub-list. Now we shall see some programming aspects of insertion sort.

## Algorithm

Now we have a bigger picture of how this sorting technique works, so we can derive simple steps by which we can achieve insertion sort.

![](./assests/picture14.png)

## Pseudocode

![](./assests/picture15.png)





