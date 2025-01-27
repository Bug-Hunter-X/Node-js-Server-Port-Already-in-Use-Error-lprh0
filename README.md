# Node.js Server Port Already in Use

This repository demonstrates a common error encountered when developing Node.js applications: attempting to start a server on a port that is already in use.  The `bug.js` file contains the problematic code, while `bugSolution.js` provides a solution.

## Problem

The provided code creates an HTTP server and attempts to listen on port 8080.  If another process (e.g., another Node.js server or a different application) is already using this port, the server will fail to start, and an error will be thrown.

## Solution

The solution involves checking if the port is available before attempting to bind to it, or implementing graceful error handling, as demonstrated in `bugSolution.js`.