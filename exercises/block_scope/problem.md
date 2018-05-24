# Exercise

Create a file named solution.js
Modify this file by choosing either `var`, `let` or `const` to make the code behave as described in the comments
Make sure to remove instruction comments

```javascript
'use strict';
// This variable `a` should be accessible outside of the block scope.
var|let|const a = 5;

// This variable `b` should not be reassignable.
var|let|const b = process.argv[2];

if (a === 5) {
  // This variable `c` should only be valid in this block.
  var|let|const c = 4;
  console.log(c);  // 4

  // This variable `b` should only be valid in this block and should not be reassignable.
  var|let|const b = 8;
  console.log(b); // 8
}

console.log(a); // 5
console.log(b);
try {
  // Trying to change the value of `c`
  c = 1000;
} catch (e) {
  // but an `c is not defined` error should occur.
  console.log(e);
}
```
