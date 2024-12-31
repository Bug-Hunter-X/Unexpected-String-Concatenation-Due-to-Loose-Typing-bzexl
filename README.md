# Unexpected String Concatenation in JavaScript

This repository demonstrates a common yet subtle bug in JavaScript related to its loose typing system.  The `foo` function is intended to add two numbers, but due to JavaScript's implicit type coercion, if one of the arguments is a string, it performs string concatenation instead of numeric addition.

## How to Reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. Observe the unexpected output (11 instead of 2).

## Solution

The `bugSolution.js` file provides a solution using explicit type checking to ensure both inputs are numbers before performing addition.  This prevents the unintended string concatenation and produces the correct result.