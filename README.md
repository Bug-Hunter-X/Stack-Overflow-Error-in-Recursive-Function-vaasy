# Stack Overflow Error in Recursive Function

This repository demonstrates a common error in JavaScript: stack overflow errors caused by unintended infinite recursion.

## Bug Description
The provided JavaScript code implements a recursive function `foo`. This function calculates the result based on the input parameters a and b. It is designed to use recursion but lacks an appropriate base case to stop the recursion for large values of 'a'. Consequently, the recursive calls will continue until the call stack is exhausted which leads to stack overflow errors. This bug mainly occurs in recursive functions when the base case is not correctly defined or handles the input values improperly.

## Bug Solution
The solution introduces a base case to terminate recursion. The function `foo` now includes a condition which properly stops recursion for appropriate input values, preventing stack overflow.

## How to reproduce
1. Clone this repository.
2. Open the `bug.js` file and run the code. Observe the Stack Overflow Error.
3. Open the `bugSolution.js` file and run the code. Observe the correct output.