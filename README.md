# Ada Out-of-Bounds Array Access Bug

This repository demonstrates a common error in Ada programming: attempting to access an array element using an index that is outside the declared bounds of the array.  This often leads to a runtime error or unexpected behavior.

## Bug Description

The Ada code in `bug.ada` tries to access an element in an array using an index that is out of bounds. This results in a runtime error because the index `Index` is set to 11, while the array `My_Array` only has elements from index 1 to 10.

## Solution

The corrected code in `solution.ada` adds a check to ensure the index is within the valid range before accessing the array element.  This prevents the out-of-bounds access and eliminates the runtime error.

## How to Reproduce

1. Compile and run `bug.ada`.  You should observe a runtime error.
2. Compile and run `solution.ada`. This version will execute without errors.