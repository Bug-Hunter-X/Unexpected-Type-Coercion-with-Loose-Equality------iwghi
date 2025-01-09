# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript bug caused by the misuse of loose equality (`==`) leading to unexpected type coercion.  Strict equality (`===`) should be preferred for most comparisons to avoid these issues.

## Bug Description
The bug arises from using loose equality (`==`) when comparing variables that might be null or undefined.  Loose equality performs type coercion, which can lead to unexpected results.

## Solution
The solution is straightforward: always use strict equality (`===`).  Strict equality does not perform type coercion, ensuring accurate comparisons. The example demonstrates how handling `null` values explicitly resolves the issue.

## How to reproduce
1. Clone the repo.
2. Run `bug.js`.  Note the unexpected output.
3. Run `bugSolution.js`.  Note the corrected output.
