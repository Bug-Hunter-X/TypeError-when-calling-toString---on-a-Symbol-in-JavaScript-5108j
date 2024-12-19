# JavaScript TypeError: Cannot convert a Symbol value to a string

This repository demonstrates a common JavaScript error: a TypeError occurring when the toString() method is called on a Symbol value.

## The Bug
The `bug.js` file contains a function `foo` that attempts to convert various data types to strings using `toString()`. However, when a Symbol is passed, a `TypeError` is thrown because Symbols don't have a default `toString()` method.

## The Solution
The `bugSolution.js` file provides a solution by adding explicit handling for Symbol values, checking the typeof the input before attempting to use toString().

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` and run it in a JavaScript environment (e.g., Node.js, a browser's console).
3. Observe the TypeError when the function receives a Symbol as input.
4. Then run `bugSolution.js` to see the fixed version handling the Symbol type.