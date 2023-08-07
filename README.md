# javascript-interview-questions

## Question 1: Find Maximum and Minimum Elements

```javascript
function findMaxAndMin(arr) {
  if (arr.length === 0) {
    throw new Error("Array is empty.");
  }

  let max = arr[0];
  let min = arr[0];

  for (let i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
      max = arr[i];
    }
    if (arr[i] < min) {
      min = arr[i];
    }
  }

  return {
    max,
    min,
  };
}

```

## Question 2: Reverse an Array In-Place

```javascript
function reverseArrayInPlace(arr) {
  let start = 0;
  let end = arr.length - 1;

  while (start < end) {
    const temp = arr[start];
    arr[start] = arr[end];
    arr[end] = temp;
    start++;
    end--;
  }
}
```

