# MongoDB $inc operator error with string value
This repository demonstrates a common error when using the `$inc` operator in MongoDB. The `$inc` operator is used to increment a numerical value in a document. However, if a non-numerical value is provided, it will result in an error.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides the corrected version.

## Error
The error occurs when providing a string value instead of a number to the `$inc` operator.  This will throw an error similar to:
```
MongoError: $inc requires a number
```
## Solution
The solution involves ensuring that the value provided to the `$inc` operator is a number.