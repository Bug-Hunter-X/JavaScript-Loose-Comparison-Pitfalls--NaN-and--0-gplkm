# JavaScript Loose Comparison Pitfalls: NaN and -0

This repository demonstrates unexpected behavior in JavaScript's loose comparison (==) operator when dealing with NaN (Not a Number) and -0 (negative zero).

## The Bug

The `foo` function intends to compare two numbers for equality using loose comparison. However, it fails for two specific cases:

1. `NaN` (Not a Number): `NaN` is never equal to itself, even using loose comparison.
2. `-0` (Negative Zero): `-0` is considered equal to `+0` using loose comparison.

## The Solution

The solution uses the strict equality operator (===) to prevent this unexpected behavior and always provides the expected results.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` to see the buggy and corrected code, respectively.
3. Run these JavaScript files in a Node.js environment, or in your browser's console.