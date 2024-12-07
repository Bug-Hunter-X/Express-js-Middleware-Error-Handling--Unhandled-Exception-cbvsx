# Express.js Middleware Error Handling: Unhandled Exception

This repository demonstrates a common yet subtle error in Express.js middleware: improper error handling that leads to server crashes. 

The `bug.js` file showcases a scenario where an exception is thrown within a middleware function, but the error isn't handled properly, causing the server process to terminate.

The `bugSolution.js` file provides the corrected implementation with appropriate error handling to gracefully manage exceptions within the middleware chain.  This prevents server crashes and allows for better error reporting to users.

## How to reproduce the bug

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js`
4. Observe the server crash and error message.

## How to fix the bug

1. Replace `bug.js` with `bugSolution.js`
2. Run `node bugSolution.js`
3. Observe the server running correctly and handling the error gracefully.