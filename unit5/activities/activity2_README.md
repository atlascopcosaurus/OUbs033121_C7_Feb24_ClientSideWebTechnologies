To modify the provided code to utilize the `switch` statement more effectively, let's change the `document.write` method to updating the inner HTML of the `<p>` element with the `id="demo"`. This approach is more dynamic and doesn't overwrite the entire HTML content of the page. Additionally, I'll adjust the variable values and demonstrate how the `switch` statement works:

```html
<!DOCTYPE html>
<html>

<head>
    <title>JavaScript Switch</title>
</head>

<body>
    <h3>Results :</h3>
    <p id="demo"></p>

    <script>
        var marks = 75; // Change this value to test different outcomes

        switch (true) {
            case (marks >= 50 && marks < 60):
                document.getElementById("demo").innerHTML = "Student got passing marks.";
                break;
            case (marks >= 60 && marks < 70):
                document.getElementById("demo").innerHTML = "Student got Good marks.";
                break;
            case (marks >= 70 && marks < 80):
                document.getElementById("demo").innerHTML = "Student got Very Good marks.";
                break;
            case (marks >= 80 && marks <= 100):
                document.getElementById("demo").innerHTML = "Student got Excellent marks.";
                break;
            default:
                document.getElementById("demo").innerHTML = "Student result not shown.";
        }
    </script>
</body>

</html>
```

In this modification:
- The variable `number` is changed to `marks` to reflect its purpose more clearly.
- The `switch` statement now evaluates `true`, making it versatile for range-based conditions instead of exact matches. This approach allows for checking ranges of values within each `case` statement.
- Each `case` checks if `marks` falls within a specific range. For example, `case (marks >= 60 && marks < 70):` checks if the marks are between 60 and 69.
- The `document.write` method is replaced with `document.getElementById("demo").innerHTML`, which updates the text of the `<p>` element with the `id="demo"` based on the student's marks. This method avoids the potential issue of `document.write` overwriting the entire HTML document after the page has loaded.
- The default case provides a message when none of the specified conditions match.

By adjusting the value of `marks`, you can see different messages displayed, demonstrating how the `switch` statement can be used for more complex conditions than just exact value matches.