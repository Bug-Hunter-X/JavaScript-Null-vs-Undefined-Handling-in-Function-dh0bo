# JavaScript Null vs. Undefined Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to how null and undefined values are handled within functions.  The initial code handles null values appropriately but neglects explicit handling of undefined inputs, leading to unexpected behavior or errors in certain scenarios.

The solution demonstrates how to properly handle both null and undefined inputs, thereby improving the robustness and reliability of the code.

## Bug

The original code in `bug.js` effectively handles null inputs, returning null in such cases. However, if undefined values are passed as arguments, the function's behavior is undefined (pun intended).  This lack of explicit error handling can lead to issues in production environments.

## Solution

The `bugSolution.js` file addresses this issue by adding checks for both null and undefined values. This ensures that the function behaves consistently and predictably regardless of the input types, thus preventing potential unexpected errors or runtime exceptions.