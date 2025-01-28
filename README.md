# Unhandled Non-numeric Input in Calculator Function

This repository demonstrates a common JavaScript bug: insufficient input validation. The `calculate` function handles addition and subtraction, but it doesn't check if the input values (`a` and `b`) are actually numbers.  It also doesn't explicitly handle potential exceptions.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides a corrected version with improved input validation and error handling.

## Bug
The original code lacks input validation. If you pass non-numeric values to the `calculate` function, it will either produce unexpected results or throw an error depending on the nature of the input.

## Solution
The solution involves adding input validation to ensure that `a` and `b` are numbers before performing the calculation.  The improved solution uses `isNaN()` to check for numbers and returns an appropriate error message if validation fails.