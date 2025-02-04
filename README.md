# Tailwind CSS Flexbox Fractional Width Issue

This repository demonstrates an unexpected behavior when using fractional widths in Tailwind CSS flexbox.

## Bug Description
When two divs are placed side-by-side using `flex`, and each is given a width of `w-1/2`, they overlap instead of taking up equal halves of the available width. This happens even when the parent div has the necessary width or is set to `flex-row`. 

## Bug Reproduction
1. Clone the repository.
2. Open the `bug.js` file.
3. Run the code. Observe the unexpected layout.

## Solution
The solution involves adding the `flex-grow` utility class.  See the `bugSolution.js` file for a fix.  This forces the elements to expand and fill the available space. 