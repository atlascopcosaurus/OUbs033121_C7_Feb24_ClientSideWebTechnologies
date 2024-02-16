### 1. Program to find the area of a triangle with sides of length 5, 6, and 7.

```javascript
// Lengths of the sides of the triangle
var side1 = 5;
var side2 = 6;
var side3 = 7;

// Calculating the semi-perimeter
var s = (side1 + side2 + side3) / 2;

// Calculating the area using Heron's formula
var area = Math.sqrt(s * (s - side1) * (s - side2) * (s - side3));

console.log("The area of the triangle is: " + area);
```

### 2. Function that converts an array element into a string.

```javascript
function arrayToString(arr) {
    return arr.toString();
    // Or use the join method for more control over the separator
    // return arr.join(", ");
}

var myArray = [1, 2, 3, 4, 5];
console.log(arrayToString(myArray)); // "1,2,3,4,5"
```

### 3. JavaScript program to demonstrate push and pop operations.

```javascript
var animals = ['Dog', 'Cat', 'Rabbit'];

console.log("Original array: ", animals.join(", "));

// Push operation
animals.push('Horse', 'Elephant');
console.log("After push operation: ", animals.join(", "));

// Pop operation
var poppedAnimal = animals.pop();
console.log("After pop operation: ", animals.join(", "));
console.log("Popped Animal: ", poppedAnimal);
```

In the first program, the formula for the area of a triangle given its three sides is applied using Heron's formula. The semi-perimeter \(s\) is first calculated, and then the area is determined using the square root function provided by `Math.sqrt`.

The second program defines a function `arrayToString` that takes an array as input and converts it into a string using the `toString()` method. This method automatically joins the array elements with commas. Alternatively, the `join()` method can be used for more control over the separator between elements.

The third program demonstrates the use of `push()` and `pop()` methods on an array. `push()` adds elements to the end of the array, while `pop()` removes the last element from the array and returns it. The state of the array is logged to the console after each operation to show the effect of these methods.