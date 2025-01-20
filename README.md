# Missing Error Handling in Express.js Route

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling when processing user input.  The provided code attempts to retrieve a user based on their ID, but it doesn't handle cases where the ID is invalid or the user isn't found. This can lead to unexpected crashes or vulnerabilities.

The `bug.js` file shows the buggy code.  The `bugSolution.js` demonstrates a corrected version with improved error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install Express.js.
3. Run `node bug.js` (you'll need a sample `users` array). Observe that it crashes if the userId is not a number or if no user is found with that ID.
4. Then run `node bugSolution.js` to see the corrected implementation.