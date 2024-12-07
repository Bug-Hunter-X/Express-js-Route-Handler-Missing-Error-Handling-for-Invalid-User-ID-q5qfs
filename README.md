# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input. Specifically, the code attempts to parse a user ID from a route parameter without checking if it's a valid number.  This can lead to unexpected behavior or crashes if the ID is not a number.

The `bug.js` file contains the flawed code, while `bugSolution.js` provides a corrected version with robust error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express` to install the required dependencies.
3. Run `node bug.js`. 
4. Access the route with an invalid ID (e.g., `/users/abc`).  Observe the error.
5. Run `node bugSolution.js` and test with a valid and invalid ID to compare the results.