# MongoDB $inc Operator with String Value
This repository demonstrates an uncommon error related to the `$inc` operator in MongoDB. The `$inc` operator is used to increment or decrement a numeric field in a document.  However, if it is provided with a non-numeric value (like a string), MongoDB will not produce an error but simply won't increment the value.

The example shows how providing a string to `$inc` leads to a failed update that is not immediately obvious.

## Solution
The solution involves ensuring the values passed to the `$inc` operator are always numbers.