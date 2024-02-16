The `splice()` function in JavaScript is a versatile method used to change the contents of an array by removing or replacing existing elements and/or adding new elements in place. Here’s a breakdown of how `splice()` works:

### Syntax
```javascript
array.splice(start[, deleteCount[, item1[, item2[, ...]]]])
```

- **start**: The index at which to start changing the array. If greater than the length of the array, actual starting index will be set to the length of the array. If negative, it will begin that many elements from the end of the array.
- **deleteCount** (Optional): An integer indicating the number of elements in the array to remove from `start`. If `deleteCount` is omitted, or if its value is greater than the number of elements left in the array starting at `start`, then all elements from `start` to the end of the array will be deleted. If `deleteCount` is 0 or negative, no elements are removed.
- **item1, item2, ...** (Optional): The elements to add to the array, beginning at the `start` index. If no elements are specified, `splice()` will only remove elements from the array.

### Example 1: Removing Elements
To remove elements from an array, you specify the index at which to start and the number of elements to remove.

```javascript
let fruits = ['Apple', 'Banana', 'Orange', 'Mango', 'Kiwi'];
// Remove 2 elements starting from index 2
fruits.splice(2, 2);

console.log(fruits); // Output: ['Apple', 'Banana', 'Kiwi']
```

### Example 2: Adding Elements
To add elements without removing any, you set `deleteCount` to 0 and specify the items to add.

```javascript
let fruits = ['Apple', 'Banana'];
// Add two elements starting from index 1, without removing any elements
fruits.splice(1, 0, 'Orange', 'Mango');

console.log(fruits); // Output: ['Apple', 'Orange', 'Mango', 'Banana']
```

### Example 3: Replacing Elements
To replace elements, you specify the index at which to start, how many elements to remove, and the new elements to add.

```javascript
let fruits = ['Apple', 'Banana', 'Kiwi'];
// Replace 1 element starting from index 1
fruits.splice(1, 1, 'Orange', 'Mango');

console.log(fruits); // Output: ['Apple', 'Orange', 'Mango', 'Kiwi']
```

### Example 4: Removing Elements from the End
By using a negative start index, you can remove elements from the end of the array.

```javascript
let fruits = ['Apple', 'Banana', 'Orange', 'Mango'];
// Remove the last 2 elements
fruits.splice(-2, 2);

console.log(fruits); // Output: ['Apple', 'Banana']
```

The `splice()` function directly modifies the array it is called on and returns an array containing the deleted elements, if any. This makes it a powerful tool for array manipulation in JavaScript.