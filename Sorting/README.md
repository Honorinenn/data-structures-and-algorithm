# data-structures-and-algorithm

1)Problem 

2 Sum In A Sorted Array
Given an array sorted in non-decreasing order and a target number, find the indices of the two values from the array that sum up to the given target number.

Example
{
"numbers": [1, 2, 3, 5, 10],
"target": 7
}
Output:

[1, 3]
Sum of the elements at index 1 and 3 is 7.

Notes
In case when no answer exists, return an array of size two with both values equal to -1, i.e., [-1, -1].
In case when multiple answers exist, you may return any of them.
The order of the indices returned does not matter.
A single index cannot be used twice.
Constraints:

2 <= Array Size <= 105.
-105 <= Array Elements <= 105.
-105 <= Target Number <= 105.
Array can contain duplicate elements.


2) Problem

2 Sum In An Array
Given an array and a target number, find the indices of the two values from the array that sum up to the given target number.

Example One
{
"numbers": [5, 3, 10, 45, 1],
"target": 6
}
Output:

[0, 4]
Sum of the elements at index 0 and 4 is 6.

Example Two
{
"numbers": [4, 1, 5, 0, -1],
"target": 10
}
Output:

[-1, -1]
Notes
The function returns an array of size two where the two elements specify the input array indices whose values sum up to the given target number.
In case when no answer exists, return an array of size two with both values equal to -1, i.e., [-1, -1].
In case when multiple answers exist, you may return any of them.
The order of the returned indices does not matter.
A single index cannot be used twice.
Constraints:

2 <= Array Size <= 105.
-105 <= Array Elements <= 105.
-105 <= Target Number <= 105.
Array can contain duplicate elements.






3) Problem
   Merge K Sorted Linked Lists
   Given k linked lists where each one is sorted in the ascending order, merge all of them into a single sorted linked list.

Example
{
"lists": [
[1, 3, 5],
[3, 4],
[7]
]
}
Output:

[1, 3, 3, 4, 5, 7]
Notes
Constraints:

0 <= k <= 104
0 <= length of any given linked list <= 103
-109 <= node values <= 109
Sum of the lengths of all given lists won't exceed 105.




4) Problem

Attend Meetings
Given a list of meeting intervals where each interval consists of a start and an end time, check if a person can attend all the given meetings such that only one meeting can be attended at a time.

Example One
{
"intervals": [[1, 5], [5, 8], [10, 15]]
}
Output:

1
As the above intervals are non-overlapping intervals, it means a person can attend all these meetings.

Example Two
{
"intervals": [[1, 5], [4, 8]]
}
Output:

0
Time 4 - 5 is overlapping in the first and second intervals.

Notes
A new meeting can start at the same time the previous one ended.
Constraints:

1 <= number of intervals <= 105
0 <= start time < end time <= 109



5) Problem

Top K Frequent Elements
Given an integer array and a number k, find the k most frequent elements in the array.

Example One
{
"arr": [1, 2, 3, 2, 4, 3, 1],
"k": 2
}
Output:

[3, 1]
Example Two
{
"arr": [1, 2, 1, 2, 3, 1],
"k": 1
}
Output:

[1]
Notes
If multiple answers exist, return any.
The order of numbers in the output array does not matter.
Constraints:

1 <= length of the given array <= 3 * 105
0 <= array element <= 3 * 105
1 <= k <= number of unique elements in the array





6)Problem

Kth Largest In A Stream

Given an initial list along with another list of numbers to be appended with the initial list and an integer k, return an array consisting of the k-th largest element after adding each element from the first list to the second list.

Example
{
"k": 2,
"initial_stream": [4, 6],
"append_stream": [5, 2, 20]
}
Output:

[5, 5, 6]
Append	Stream	Sorted Stream	2nd largest
5	[4, 6, 5]	[4, 5, 6]	5
2	[4, 6, 5, 2]	[2, 4, 5, 6]	5
20	[4, 6, 5, 2, 20]	[2, 4, 5, 6, 20]	6
Notes
The stream can contain duplicates.
Constraints:

1 <= length of both lists <= 105.
1 <= k <= length of initial list + 1.
0 <= any value in the list <= 109.



7) Problem

Kth Largest In An Array
Given an array of integers, find the k-th largest number in it.

Example One
{
"numbers": [5, 1, 10, 3, 2],
"k": 2
}
Output:

5
Example Two
{
"numbers": [4, 1, 2, 2, 3],
"k": 4
}
Output:

2
Notes
Constraints:

1 <= Array Size <= 3*105.
-109 <= Array Elements <= 109.
1 <= k <= Array Size.



8) Problem


Online Median
Given a list of numbers, the task is to insert these numbers into a stream and find the median of the stream after each insertion. If the median is a non-integer, consider it’s floor value.

The median of a sorted array is defined as the middle element when the number of elements is odd and the mean of the middle two elements when the number of elements is even.

Example
{
"stream": [3, 8, 5, 2]
}
Output:

[3, 5, 5, 4]
Iteration	Stream	Sorted Stream	Median
1	[3]	[3]	3
2	[3, 8]	[3, 8]	(3 + 8) / 2 => 5
3	[3, 8, 5]	[3, 5, 8]	5
4	[3, 8, 5, 2]	[2, 3, 5, 8]	(3 + 5) / 2 => 4
Notes
Constraints:

1 <= length of stream <= 105
1 <= any value in the stream <= 105
The stream can contain duplicates.





9) Problem

Intersection Of Three Sorted Arrays
Given three arrays sorted in the ascending order, return their intersection sorted array in the ascending order.

Example One
{
"arr1": [2, 5, 10],
"arr2": [2, 3, 4, 10],
"arr3": [2, 4, 10]
}
Output:

[2, 10]
Example Two
{
"arr1": [1, 2, 3],
"arr2": [],
"arr3": [2, 2]
}
Output:

[-1]
Example Three
{
"arr1": [1, 2, 2, 2, 9],
"arr2": [1, 1, 2, 2],
"arr3": [1, 1, 1, 2, 2, 2]
}
Output:

[1, 2, 2]
Notes
If the intersection is empty, return an array with one element -1.
Constraints:

0 <= length of each given array <= 105
0 <= any value in a given array <= 2 * 106















PROBLEM SET 1 FOR SORTING

1) Problem


Segregate Even And Odd Numbers
Given an array of numbers, rearrange them in-place so that even numbers appear before odd ones.

Example
{
"numbers": [1, 2, 3, 4]
}
Output:

[4, 2, 3, 1]
The order within the group of even numbers does not matter; same with odd numbers. So the following are also correct outputs: [4, 2, 1, 3], [2, 4, 1, 3], [2, 4, 3, 1].

Notes
It is important to practice solving this problem by rearranging numbers in-place.
There is no need to preserve the original order within the even and within the odd numbers.
We look for a solution of the linear time complexity that uses constant auxiliary space.
Constraints:

1 <= length of the array <= 105
1 <= element of the array <= 109





2) Problem

Implement Merge Sort
Given a list of numbers, sort it using the Merge Sort algorithm.

Example
{
"arr": [5, 8, 3, 9, 4, 1, 7]
}
Output:

[1, 3, 4, 5, 7, 8, 9]
Notes
Constraints:

1 <= length of the given list <= 105
-109 <= number in the list <= 109



3) Problem


Merge One Sorted Array Into Another
First array has n positive numbers, and they are sorted in the non-descending order.

Second array has 2n numbers: first n are also positive and sorted in the same way but the last n are all zeroes.

Merge the first array into the second and return the latter. You should get 2n positive integers sorted in the non-descending order.

Example
{
"first": [1, 3, 5],
"second": [2, 4, 6, 0, 0, 0]
}
Output:

[1, 2, 3, 4, 5, 6]
Notes
Constraints:

1 <= n <= 105
1 <= array elements (except those zeroes) <= 2 * 109
You can use only constant auxiliary space
