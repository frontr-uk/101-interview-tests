Given a list of non negative integers, arrange them in such a manner that they form the largest number possible.The result is going to be very large, hence return the result in the form of a string.

Example 1:

Input:

N = 5
Arr[] = {3, 30, 34, 5, 9}

Output: 9534330

Explanation: Given numbers are {3, 30, 34,5, 9}, the arrangement 9534330 gives the largest value.

```
function test(arr){
    return arr.map(String).sort((a, b) => (b + a) - (a + b)).join('')
}

console.log(test([3, 30, 34, 5, 9]))
```
