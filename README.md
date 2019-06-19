#What

```js
var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

var result1 = arr.map(getSquare);
console.log(`result1 @ ${getTime()}`, result1);

var result2 = await arr.asyncMapPool(getSquareAsync, 1);
console.log(`result2 @ ${getTime()}`, result2);

var result3 = await arr.asyncMapS(getSquareAsync);
console.log(`result3 @ ${getTime()}`, result3);

var result4 = arr.reduce(getArraySum, 0);
console.log(`result4 @ ${getTime()} - Sum is`, result4);

var result5 = await arr.asyncReduce(getArraySumAsync, 0);
console.log(`result5 @ ${getTime()} - Sum is`, result5);
```
