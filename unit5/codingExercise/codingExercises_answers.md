### 1. Output of the given code:

The given code snippet will set `y` as a global variable because it is not declared with `var`, `let`, or `const` inside the function (assuming strict mode is not enabled). The variable `x` is declared locally within the function and will not be accessible outside of it. Thus, the output will be the value assigned to `y`, which is `5`. However, without the complete HTML context or assuming `demo` is an existing element's ID, this explanation assumes `document.getElementById("demo").innerHTML = y;` correctly targets an element.

### 2. JavaScript code to check if the temperature of the last five days goes below zero:

```javascript
const temperatures = [-3, 1, 0, -5, 2]; // Example temperatures of the last five days

function checkTemperature(temps) {
    for (let i = 0; i < temps.length; i++) {
        if (temps[i] < 0) {
            console.log(`Temperature went below zero on day ${i + 1} with ${temps[i]}°C.`);
        }
    }
}

checkTemperature(temperatures);
```

### 3. JavaScript code using a for loop to print odd numbers from 50-100:

```javascript
for (let number = 51; number <= 100; number += 2) { // Starting from 51 to ensure it's odd and increment by 2
    console.log(number);
}
```

### 4. JavaScript code using a while loop that prints prime numbers from 100-150:

```javascript
function isPrime(num) {
    for (let i = 2, sqrt = Math.sqrt(num); i <= sqrt; i++)
        if (num % i === 0) return false;
    return num > 1;
}

let number = 100;
while (number <= 150) {
    if (isPrime(number)) {
        console.log(number);
    }
    number++;
}
```

### 5. Modifying an admission form with validation techniques:

Assuming the form includes elements like name, email, and age, here's a basic example of how you might apply validation techniques:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Admission Form Validation</title>
</head>
<body>
    <form id="admissionForm">
        Name: <input type="text" id="name" required>
        Email: <input type="email" id="email" required>
        Age: <input type="number" id="age" min="18" required>
        <button type="submit">Submit</button>
    </form>

    <script>
        document.getElementById("admissionForm").onsubmit = function(event) {
            event.preventDefault(); // Prevent form submission to see console output

            const name = document.getElementById("name").value;
            const email = document.getElementById("email").value;
            const age = parseInt(document.getElementById("age").value, 10);

            if (name.trim() === "") {
                alert("Name is required.");
                return;
            }

            if (email.trim() === "") {
                alert("Email is required.");
                return;
            }

            if (isNaN(age) || age < 18) {
                alert("You must be at least 18 years old.");
                return;
            }

            console.log("Form is valid. Name:", name, "Email:", email, "Age:", age);
            // Here you would typically submit the form or do further processing
        };
    </script>
</body>
</html>
```

This example checks that the form's inputs are not empty (or in the case of age, not below 18) and prevents form submission if any of the validation checks fail. Real-world applications would likely require more comprehensive validations.