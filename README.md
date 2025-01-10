# Node.js HTTP Server Unhandled Exception

This repository demonstrates a common error in Node.js HTTP servers:  lack of proper error handling.  The `bug.js` file shows a server vulnerable to crashes, while `bugSolution.js` provides a corrected version.

**Problem:**
The original server doesn't handle potential errors during request processing.  This makes it susceptible to crashing if an error occurs within the request handler.

**Solution:**
The improved version incorporates a `try...catch` block to gracefully handle exceptions, preventing the server from crashing.  It logs the error for debugging purposes and sends an appropriate error response to the client.

This demonstrates best practices for building robust and reliable Node.js applications.