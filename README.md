# Unhandled Asynchronous Errors in Node.js

This repository demonstrates a common error in Node.js applications: unhandled errors within asynchronous operations, specifically in an Express.js server.  The `bug.js` file contains code that simulates an asynchronous operation (using `setTimeout`) that can throw an error. If the random number generated is less than 0.5, an error is thrown, causing the server to crash without proper error handling.

The `bugSolution.js` file provides a solution by properly handling the error using a `try...catch` block or by using promises and `.catch()` method. This ensures graceful error handling and prevents the application from crashing.