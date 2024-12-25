# CSS `calc()` Unit Mismatch

This repository demonstrates a subtle error that can occur when using the `calc()` function in CSS.  The issue arises from mixing percentage and absolute units within a single calculation.

## The Problem
The `calc()` function in CSS allows you to perform calculations to determine property values.  However, it's crucial to maintain consistent units within each calculation.  Mixing percentage units with absolute units (like `px`, `em`, `rem`, etc.) often leads to unexpected results or parsing errors.

## Reproducing the Error
The `bug.css` file contains CSS code that reproduces this error. The `height` property uses `calc()` with a mixture of percentage and `em` units.

## Solution
The `bugSolution.css` file provides a corrected version. The solution involves ensuring consistent units within each `calc()` expression.  You could use only percentages or only absolute units to resolve this problem.

## How to use it
1. Clone this repository.
2. Open `bug.html` (or a similar HTML file) in your browser to observe the error.
3. Compare the CSS in `bug.css` with the corrected version in `bugSolution.css`.