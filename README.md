# MongoDB $inc Operator Type Error
This example demonstrates an error in using the MongoDB $inc operator.  The `$inc` operator is used to increment a numerical field in a document.  Using a string instead of a number will lead to an unexpected result; the counter will not increment correctly. The solution shows the correct usage with a numerical value.

## How to Reproduce
1. Connect to a MongoDB instance.
2. Create a collection with a document containing a numerical field (e.g., `count`).
3. Run the `bug.js` script.  Observe the value of the `count` field after execution.
4. Run the `bugSolution.js` script and observe the correct behavior. 

## Solution
The solution involves using a numerical value instead of a string with the `$inc` operator.