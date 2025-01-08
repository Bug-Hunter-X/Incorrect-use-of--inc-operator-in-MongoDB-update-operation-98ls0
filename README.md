# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field.  However, if a string is provided as the increment value, unexpected behavior occurs.

## Bug Description

The provided code incorrectly uses a string ("1") as the increment value for the `counter` field. This results in a failure to increment the field properly.

## Solution

The solution involves providing a number (1) as the increment value to correctly increment the counter field.  See the `bugSolution.js` file for the corrected implementation.

## How to Reproduce

1.  Clone this repository.
2.  Connect to your MongoDB instance.
3.  Run `bug.js`. Observe the incorrect result.
4.  Run `bugSolution.js`. Observe the correct result.
