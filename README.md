# Sum-of-two-lowest-postive-integers

## Problem

Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers. No floats or non-positive integers will be passed.

For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.

[10, 343445353, 3453445, 3453545353453] should return 3453455.

FUNDAMENTALSARRAYS
Suggest kata description edits

```javascript

const sumTwoSmallestNumbers = (numbers) => {
// assign a variable to sort numbers
  var orderList = numbers.sort((a,b) => a - b);
//   assign a acc
  var add = 0;
//   for-loop
 for(i=0; i< orderList.length; i++) {
   if(i==0) {
    add += orderList[0];
   }
   if(i==1) {
     add += orderList[1];
   }
 }
  return add;
 };
```
