# CSS Calc() Percentage Subtraction Bug

This repository demonstrates a subtle bug related to using the `calc()` function in CSS.  Specifically, it highlights the unexpected behavior when attempting to subtract a percentage value from a fixed-length value (like pixels) directly inside the `calc()` function.

The `bug.css` file contains the problematic code.  The `bugSolution.css` file provides the correct way to achieve the intended behavior.

## Reproducing the Bug

1. Open `bug.html` (a simple HTML file containing a div with the problematic CSS) in a web browser.
2. Observe the rendered width of the div.  It might not be what you expect.

## Solution

The solution requires explicitly calculating the percentage before subtracting from the fixed length value. See `bugSolution.css` for details.

## Browser Compatibility

While `calc()` has good support, the specific behavior of percentage subtraction from pixel values might vary slightly between browsers.