# MongoDB $inc operator error
This example demonstrates an incorrect usage of the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided instead of a number, the update operation will either fail or produce an unexpected result.

## Bug
The bug lies in the incorrect usage of the `$inc` operator: `{$inc: {field: '1'}}` should be  `{$inc: {field: 1}}`.

## Solution
The solution involves correcting the update operation to correctly use a numeric value with the `$inc` operator.