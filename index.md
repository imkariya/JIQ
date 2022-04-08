## Question1.
A bracket is considered to be any one of the following characters: (, ), {, }, [, or ].
Two brackets are considered to be a matched pair if the opening bracket (i.e., (, [, or {) occurs to the left of a closing bracket (i.e., ), ], or }) of the exact same type. There are three types of matched pairs of brackets: [], {}, and ().
A matching pair of brackets is not balanced if the set of brackets it encloses are not matched. For example, {[(])} is not balanced because the contents in between { and } are not balanced. The pair of square brackets encloses a single, unbalanced opening bracket, (, and the pair of parentheses encloses a single, unbalanced closing square bracket, ].
By this logic, we say a sequence of brackets is balanced if the following conditions are met:
It contains no unmatched brackets.
The subset of brackets enclosed within the confines of a matched pair of brackets is also a matched pair of brackets.
Given  strings of brackets, determine whether each sequence of brackets is balanced. If a string is balanced, return YES. Otherwise, return NO.
Function Description
Complete the function isBalanced in the editor below.
isBalanced has the following parameter(s):
string s: a string of brackets
Returns
string: either YES or NO
Input Format
The first line contains a single integer , the number of strings.
Each of the next  lines contains a single string , a sequence of brackets
, where  is the length of the sequence.
All characters in the sequences ∈ { {, }, (, ), [, ] }.
Output Format
For each string, return YES or NO.

`Sample Input`
```js
STDIN           Function
-----           --------
3               n = 3
{[()]}          first s = '{[()]}'
{[(])}          second s = '{[(])}'
{{[[(())]]}}    third s ='{{[[(())]]}}'
```
`Sample Output`
```
YES
NO
YES
```
Explanation
The string {[()]} meets both criteria for being a balanced string.
The string {[(])} is not balanced because the brackets enclosed by the matched pair { and } are not balanced: [(]).
The string {{[[(())]]}} meets both criteria for being a balanced string.































## Question 2.
Given a matrix of size r*c. Traverse the matrix in spiral form.
Example 1:
`Input:`
```
r = 4, c = 4
matrix[][] = {{1, 2, 3, 4},
           {5, 6, 7, 8},
           {9, 10, 11, 12},
           {13, 14, 15,16}}
```           
`Output:` 
```
1 2 3 4 8 12 16 15 14 13 9 5 6 7 11 10
```
![original1](https://user-images.githubusercontent.com/97151477/162397521-0ac0aa7e-acd4-4510-9b62-f40755df042f.png)


Example 2:
`Input:`
```
r = 3, c = 4  
matrix[][] = {{1, 2, 3, 4},
           {5, 6, 7, 8},
           {9, 10, 11, 12}}
```           
`Output:`
```
1 2 3 4 8 12 11 10 9 5 6 7
```
`Explanation:`
Applying same technique as shown above, 
output for the 2nd test case will be 
1 2 3 4 8 12 11 10 9 5 6 7.

 
`Your Task:`
```
You don't need to read input or print anything. Complete the function spirallyTraverse() that takes matrix, r and c as input parameters and returns a list of integers denoting the spiral traversal of matrix. 
Question 3.-> You are given a number N. Find the total count of set bits for all numbers from 1 to N(both inclusive).
```


## Question 3.
You are given a number N. Find the total count of set bits for all numbers from 1 to N(both inclusive).
 
Example 1:
`Input:` N = 4
```
`Output:` 5
```
`Explanation:`
```
For numbers from 1 to 4.
For 1: 0 0 1 = 1 set bits
For 2: 0 1 0 = 1 set bits
For 3: 0 1 1 = 2 set bits
For 4: 1 0 0 = 1 set bits
Therefore, the total set bits is 5.
 
Example 2:
`Input:` N = 17
```
`Output:` 35
```
`Explanation:`
```
From numbers 1 to 17(both inclusive), 
The total number of set bits is 35.
 
`Your Task:` 
```
The task is to complete the function countSetBits() that takes n as a parameter and returns the count of all bits.
```
 
 
 
 
 
 
## Question 4.
Given an array A of n positive numbers. The task is to find the first Equilibrium Point in the array. 
Equilibrium Point in an array is a position such that the sum of elements before it is equal to the sum of elements after it.
Note: Return the index of Equilibrium point. (1-based index)
`Example 1:`
`Input:`
``` 
n = 5 
A[] = {1,3,5,2,2} 
Output: 3 
```
`Explanation:`
```
For second test case 
equilibrium point is at position 3 
as elements before it (1+3) = 
elements after it (2+2). 
 
 
`Example 2:`
`Input:`
n = 1
A[] = {1}
Output: 1
Explanation:
Since its the only element hence
it's the only equilibrium point.
 
`Your Task:`
The task is to complete the function equilibriumPoint() which takes the array and n as input parameters and returns the point of equilibrium. Return -1 if no such point exists.




```



# Question 5
##### Given a square matrix, the task is that we turn it by 180 degrees in an anti-clockwise direction without using any extra space. 
Examples : 
```js
Input :  1  2  3
         4  5  6
         7  8  9
```
```js
Output : 9 8 7 
         6 5 4 
         3 2 1
```
```js
Input :  1 2 3 4 
         5 6 7 8 
         9 0 1 2 
         3 4 5 6 
```
```js
Output : 6 5 4 3 
         2 1 0 9 
         8 7 6 5 
         4 3 2 1
```


# Question 6
#####  Given an unsorted array of integers, sort the array into a wave like array. An array ‘arr[0..n-1]’ is sorted in wave form if arr[0] >= arr[1] <= arr[2] >= arr[3] <= arr[4]

Example
```js
Input:  arr[] = {10, 5, 6, 3, 2, 20, 100, 80}
```
```js
 Output: arr[] = {10, 5, 6, 2, 20, 3, 100, 80} OR
                 {20, 5, 10, 2, 80, 6, 100, 3} OR
                 any other array that is in wave form
```

```js
10		6		20		100
	5		2		3			80
```

```js
Input:  arr[] = {2, 4, 6, 8, 10, 20}
```
```js
 Output: arr[] = {4, 2, 8, 6, 20, 10} OR
                 any other array that is in wave form
```
```js
 Input:  arr[] = {3, 6, 5, 10, 7, 20}
 ```
 ```js
 Output: arr[] = {6, 3, 10, 5, 20, 7} OR
                 any other array that is in wave form
```




# Question 7
#####  A frog is crossing a river. The river is divided into x units and at each unit there may or may not exist a stone. The frog can jump on a stone, but it must not jump into the water.
##### Given a list of stones’ positions (in units) in sorted ascending order, determine if the frog is able to cross the river by landing on the last stone. Initially, the frog is on the first stone and assume the first jump must be 1 unit.
##### If the frog’s last jump was k units, then its next jump must be either k — 1, k, or k + 1 units. Note that the frog can only jump in the forward direction.
```js
Constraints :

2≤Number of Stones<1100
Each Stone’s position will be a non negative value < 2³¹
1st stone’s position is always 0.

Example :
[0,1,3,5,6,8,12,17]

There are a total of 8 stones.
The first stone at the 0th unit, second stone at the 1st unit,
third stone at the 3rd unit, and so on...
The last stone at the 17th unit.

Return true. The frog can jump to the last stone by jumping
1 unit to the 2nd stone, then 2 units to the 3rd stone, then
2 units to the 4th stone, then 3 units to the 6th stone,
4 units to the 7th stone, and 5 units to the 8th stone.
```


# Question 8
##### Partition problem is to determine whether a given set can be partitioned into two subsets such that the sum of elements in both subsets is the same. 
```js
Examples: 
arr[] = {1, 5, 11, 5}
Output: true 
The array can be partitioned as {1, 5, 5} and {11}
```
```js
arr[] = {1, 5, 3}
Output: false 
The array cannot be partitioned into equal sum sets.
```

# Question 9

##### Minimum number of deletion in a string to make it a palindrome
```js
Input : aebcbda
Output : 2
Remove characters 'e' and 'd'
Resultant string will be 'abcba'
which is a palindromic string
```

# Question 6
##### Given an array which is sorted, but after sorting some elements are moved to either of the adjacent positions, i.e., arr[i] may be present at arr[i+1] or arr[i-1]. Write an efficient function to search an element in this array. Basically the element arr[i] can only be swapped with either arr[i+1] or arr[i-1].


```js
For example consider the array {2, 3, 10, 4, 40}, 4 is moved to next position and 10 is moved to previous position.
```
```js
* HINT -Efficient Program ,user should use Binary Search approach
```

```js
Example : 
 
Input: arr[] =  {10, 3, 40, 20, 50, 80, 70}, key = 40
Output: 2 
Output is index of 40 in given array

Input: arr[] =  {10, 3, 40, 20, 50, 80, 70}, key = 90
Output: -1
-1 is returned to indicate element is not present
```

# Question 10
##### Given a Positive Number. Find The Number is even or odd without using Modulus(%) or Divide(/).


# Question 11

##### Given N lines and one starting point and destination point in 2-dimensional space. These N lines divide the space into some blocks. We need to print the minimum number of jumps to reach destination point from starting point. We can jump from one block to other block only if they share a side.

```js
Examples:
Input : Lines = [x = 0, y = 0, x + y – 2 = 0]
        Start point = [1, 1], 
        Dest point  = [-2, -1]
Output : 2    
```
```js
We need to jump 2 times (B4 -> B3 then B3 -> B5 
or B4 -> B6 then B6 -> B5) to reach destination 
point from starting point shown in below diagram. 
Each block i is given an id Bi in the diagram.


```
![SpaceByBlock](https://user-images.githubusercontent.com/59438970/162400479-7795db52-339c-4592-aec9-7bff05546e1c.jpg)



