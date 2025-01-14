# MongoDB $inc Operator Error: Unexpected String Increment
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  Incorrectly using a string value instead of a numerical value with `$inc` leads to the `counter` field being appended with the string, rather than being incremented numerically.  The solution shows the correct implementation.

## Bug
The `bug.js` file shows an example of incorrectly using the `$inc` operator, resulting in unexpected data modification.

## Solution
The `bugSolution.js` file demonstrates the correct usage of the `$inc` operator, ensuring numerical increments.

## How to reproduce the bug
1. Setup a MongoDB instance
2. Create a collection named 'myCollection' with a document containing a field called 'counter'
3. Run the code in `bug.js`
4. Check the value of the 'counter' field in the database. It will not be numerically incremented. 
