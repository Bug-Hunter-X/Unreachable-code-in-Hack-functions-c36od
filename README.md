# Unreachable Code in Hack

This repository demonstrates a scenario where unreachable code in Hack functions is not detected by the compiler.  The example highlights a potential issue for developers working with larger codebases, as this could lead to unnoticed bugs and inefficiencies.  The `bug.hack` file contains the problematic code; `bugSolution.hack` demonstrates a refactoring to improve readability and eliminate the unreachable code.

## Problem

The `baz` function in `bug.hack` contains a commented-out section of code. While this is intended in this example, a more substantial or complex scenario could produce dead or unreachable code accidentally.  Ideally, the compiler would issue a warning for this, ensuring that developers are aware of potential issues.  The lack of warning contributes to the difficulty in maintaining and refactoring larger Hack projects.

## Solution

The solution, in `bugSolution.hack`, removes the unnecessary code.  A more robust solution in a real-world scenario might require using code analysis tools beyond the compiler's capabilities to more effectively detect unreachable code, particularly in intricate control flows.

## Running the Code

1. Ensure you have the Hack compiler set up.
2. Compile and run the `bug.hack` and `bugSolution.hack` files using the Hack compiler.