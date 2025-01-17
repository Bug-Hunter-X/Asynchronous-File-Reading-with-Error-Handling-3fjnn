# Asynchronous File Reading with Error Handling in Node.js

This example demonstrates how to read a file asynchronously in Node.js using `fs.promises` and handle potential errors, specifically the `ENOENT` error (file not found).

## Problem

Reading files asynchronously is crucial for avoiding blocking the main thread.  However, improper error handling can lead to unexpected behavior or crashes.

## Solution

The provided code uses `async/await` to handle the asynchronous operation elegantly.  It includes a `try...catch` block to capture any errors that occur during file reading.  The code specifically checks for the `ENOENT` error and logs a user-friendly message if the file is not found.  Other errors are also caught and logged for debugging purposes.

## How to Run

1. Save the code as `bug.js`.
2. Create a file named `myFile.txt` (or modify the file path in the code) in the same directory.
3. Run the script from your terminal: `node bug.js`