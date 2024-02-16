1. **Difference between Java and JavaScript:**
   - **Java** is a statically typed, class-based programming language designed for building standalone applications or server-side applications. It requires compilation into bytecode, which runs on any device equipped with a Java Virtual Machine (JVM).
   - **JavaScript** is a dynamically typed, prototype-based scripting language primarily used for building interactive web applications. It runs directly in web browsers without the need for compilation. Despite the similarity in names, Java and JavaScript are distinct languages with different syntax, concepts, and use cases.

2. **Why is JavaScript called the Client-Side Scripting language?**
   JavaScript is termed a client-side scripting language because it is predominantly used to write scripts that run in the web browser (client-side), as opposed to the server-side. These scripts can manipulate web page content, respond to user actions, validate forms, etc., without needing to communicate with the server for every action, providing a smoother user experience.

3. **How are variables defined in JavaScript?**
   Variables in JavaScript are defined using the `var`, `let`, or `const` keywords. `var` is function-scoped or globally-scoped, `let` and `const` are block-scoped, and `const` is used for variables whose values are not intended to change.
   Examples:
   ```javascript
   var name = "John";
   let age = 30;
   const birthday = "January 1";
   ```

4. **How are comments added in JavaScript code?**
   Comments in JavaScript are added using:
   - Single-line comments, starting with `//`
     Example: `// This is a single-line comment`
   - Multi-line comments, enclosed between `/*` and `*/`
     Example:
     ```javascript
     /*
      This is a
      multi-line comment
     */
     ```

5. **What would be the result of 3+2+”7″?**
   The result would be `"57"`. JavaScript performs addition from left to right. The numbers 3 and 2 are added arithmetically to get 5. Then, 5 is concatenated with the string "7" to produce the string "57".

6. **Difference between local and global variables:**
   - **Local variables** are declared within a function and are accessible only within that function, not outside it. Their scope is limited to the function or block in which they are defined.
   - **Global variables** are declared outside any function or declared within a function without using `var`, `let`, or `const` (in non-strict mode), making them accessible from any part of the program.

7. **Short note on JavaScript Functions:**
   Functions in JavaScript are blocks of code designed to perform a particular task and are executed when "invoked" or "called". They can take parameters, perform actions with those parameters, and return a result. Functions can be defined using the function declaration or expression, and they provide a way to structure your code, make it reusable, and manage its execution flow. JavaScript also supports anonymous functions and arrow functions introduced in ES6.

8. **Explain push and pop methods in JavaScript:**
   - **push() method**: Adds one or more elements to the end of an array and returns the new length of the array. This method modifies the original array.
     Example: `arr.push('new element')`
   - **pop() method**: Removes the last element from an array and returns that element. This method changes the length of the array and modifies the original array.
     Example: `var lastElement = arr.pop()`