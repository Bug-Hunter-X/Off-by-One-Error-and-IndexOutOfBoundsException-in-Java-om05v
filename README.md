# Java Off-by-One Error and IndexOutOfBoundsException

This repository demonstrates a common Java programming error: an off-by-one error leading to an `IndexOutOfBoundsException`. The `Bug.java` file contains the erroneous code, while `BugSolution.java` provides the corrected version.

**Bug Description:**

The original code attempts to iterate through an array using a loop condition `i <= arr.length`. This causes the loop to run one iteration too many, resulting in an attempt to access an element beyond the array's bounds.  Additionally, the code then attempts to access arr[5] which is out of bounds even if the loop were corrected.

**Solution:**

The solution in `BugSolution.java` corrects the loop condition to `i < arr.length` preventing the off-by-one error and avoids accessing any elements beyond the defined length of the array.  It also addresses the attempt to access an invalid array index.