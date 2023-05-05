Download Link: https://assignmentchef.com/product/solved-datastructure-homework6-sorting
<br>
For this assignment you will be coding 4 different sorts: bubble sort, insertion sort, merge sort, and LSD radix sort. In addition to the requirements for each sort, we will be looking at the number of comparisons made between elements while grading.

<strong>Your implementations must match what was taught in lecture and recitation to receive credit. </strong>Implementing a different sort or a different implementation for a sort will receive no credit even if it passes comparison checks.

<h2>Comparator</h2>

Each sorting method (except radix sort) will take in a comparator and use it to sort the elements of the array using various sorting algorithms described below and in the sorting file. You <strong>must </strong>use this comparator as the number of comparisons performed with it will be used when testing your assignment. Note that comparator.compare(<em>x</em>, <em>y</em>) is equivalent to <em>x</em>.compareTo(<em>y</em>).

The comparison counts given in the student tests should give you an idea of what types of comparison counts you should be getting.

<h2>Inplace Sorts</h2>

An inplace sort means that the items in the array passed in aren’t copied over to another data structure in the process. Note that you can still create variables that hold only one item; you cannot create another data structure such as an array or list in the method.

<h2>Stable Sorts</h2>

A stable sort means that duplicates should remain in the same relative positions after sorting as they were before sorting.

<strong>Adaptive Sorts</strong>

An adaptive sort means that the algorithm takes advantage of existing order in the array.

<h2>Bubble Sort</h2>

Bubble sort should be inplace, stable, and adaptive. It should have a worst case running time of <em>O</em>(<em>n</em><sup>2</sup>) and a best case running time of <em>O</em>(<em>n</em>).

<h2>Insertion Sort</h2>

Insertion sort should be inplace, stable, and adaptive. It should have a worst case running time of <em>O</em>(<em>n</em><sup>2</sup>) and a best case running time of <em>O</em>(<em>n</em>).

Note that, for this implementation, you should sort from the beginning of the array. This means that after the first pass, index 0 and 1 should be considered as sorted. After the second pass, index 0-2 should be considered as sorted. After the third pass, index 0-3 should be considered as sorted, and so on.

<h2>Merge Sort</h2>

Merge sort should be stable. It should have a worst case running time of <em>O</em>(<em>n</em>log<em>n</em>) and a best case running time of <em>O</em>(<em>n</em>log<em>n</em>).

<h2>Radix Sort</h2>

Radix sort should be stable. It should have a worst case running time of <em>O</em>(<em>kn</em>) and a best case running time of <em>O</em>(<em>kn</em>), where <em>k </em>is the number of digits in the longest number. You will be implementing the least significant digit version of the sort. You will be sorting ints. Note that you CANNOT change the ints into Strings at any point in the sort for this exercise. The sort <strong>must </strong>be done in base 10. Also, as per the forbidden statements section, you cannot use anything from the Math class besides Math.abs(). However, be wary of handling overflow if you use Math.abs()!