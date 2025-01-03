# Unhandled Promise Rejections in Node.js Express Server

This repository demonstrates a common issue in Node.js Express servers: unhandled promise rejections.  The example showcases a server that introduces a delay before sending a response.  If the client times out before the response is received, it will lead to a potentially overlooked error.

## The Problem

The `bug.js` file contains an Express server that simulates a 5-second delay before sending a response.  This delay can cause problems if a client requests a response and times out before the delay completes.

## The Solution

The `bugSolution.js` file shows how to handle potential errors and properly manage asynchronous operations.  It adds error handling to prevent unhandled promise rejections.