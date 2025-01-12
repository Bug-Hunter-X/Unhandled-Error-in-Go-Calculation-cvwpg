# Unhandled Error in Go Calculation

This example demonstrates a common error in Go: not checking the return value of a function that might return an error. The `Calculate` function correctly returns an error if it tries to divide by zero, but the `main` function fails to handle this error, potentially leading to unexpected behavior or a panic.

## Bug

The `bug.go` file contains the buggy code. The `Calculate` function correctly handles division by zero by returning an error. However, the `main` function does not check for this error, leading to the unhandled error condition.

## Solution

The `bugSolution.go` file shows how to correct this. The `main` function now explicitly checks the `err` value returned by `Calculate`. If an error occurred, it prints an error message; otherwise, it prints the result.

This showcases the importance of diligently handling errors in Go to create robust and reliable applications.