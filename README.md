# Uncommon Java Bug: ArrayIndexOutOfBoundsException

This repository demonstrates a subtle and often overlooked cause of `ArrayIndexOutOfBoundsException` in Java. The bug is rooted in an off-by-one error in a loop's conditional statement.

## The Bug
The `bug.java` file contains the buggy code. The `for` loop's condition `i <= arr.length` incorrectly iterates one element past the array's bounds, leading to an exception when `i` becomes 5.

## The Solution
The `bugSolution.java` file provides the corrected code.  The loop condition is changed to `i < arr.length` ensuring that the loop iterates within the valid index range of the array. 

This example highlights the importance of careful attention to loop conditions when working with arrays in Java.