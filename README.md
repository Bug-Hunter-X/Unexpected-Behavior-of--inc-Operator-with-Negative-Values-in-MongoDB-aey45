# Unexpected Behavior of $inc Operator with Negative Values in MongoDB

This repository demonstrates a potential issue when using the `$inc` operator in MongoDB update queries with negative values.  The problem arises when the initial value of the counter is 0; a negative increment results in a negative value, which might not be the desired outcome in many scenarios.

The `bug.js` file showcases the incorrect usage.  The `bugSolution.js` file demonstrates the improved approach, handling the case where the counter is 0.