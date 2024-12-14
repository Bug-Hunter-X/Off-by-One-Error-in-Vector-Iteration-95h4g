# Off-by-One Error in Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a vector using a for loop.  The error results in accessing an element beyond the valid range of the vector, leading to undefined behavior.  The solution shows how to correctly iterate to avoid the error.

## Bug

The `bug.cpp` file contains the erroneous code. The loop condition `i <= vec.size()` causes the loop to iterate one time too many. 

## Solution

The `bugSolution.cpp` file provides the corrected code with the loop condition changed to `i < vec.size()` ensuring the loop terminates before accessing an invalid index.  The vector's size is 5; therefore, the valid indices are 0 to 4 (inclusive).