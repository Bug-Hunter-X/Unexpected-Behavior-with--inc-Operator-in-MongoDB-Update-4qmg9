# Unexpected Behavior with $inc Operator in MongoDB Update
This example demonstrates a potential issue when using the `$inc` operator in MongoDB updates.  The problem arises from incorrect usage or unintended consequences.  The solution showcases the correct method for decrementing a field using `$inc` and explains how to handle potential errors.

## Bug
The original code attempts to decrement a counter field using `$inc` with a negative value. However, potential issues arise if the counter field does not exist or is not a number. This may result in unexpected behavior or errors.

## Solution
The improved code includes error handling and verification to ensure the `$inc` operator works correctly.  It checks that the field exists and is numeric before attempting to decrement it.