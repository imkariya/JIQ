## Question 1.
Given a matrix of size r*c. Traverse the matrix in spiral form.

`Input:`
```
r = 4, c = 4
matrix[][] = {{1, 2, 3, 4}, {5, 6, 7, 8}, {9, 10, 11, 12}, {13, 14, 15,16}}
```           
`Output:` 
```
1 2 3 4 8 12 16 15 14 13 9 5 6 7 11 10
```
![original1](https://user-images.githubusercontent.com/97151477/162397521-0ac0aa7e-acd4-4510-9b62-f40755df042f.png)




# Question 2
##### Given a square matrix, the task is that we turn it by 180 degrees in an anti-clockwise direction without using any extra space. 
Examples : 

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




# Question 3

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


