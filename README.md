# Unhandled Exception in Groovy Closure

This repository demonstrates a common issue in Groovy where exceptions thrown within closures are not properly handled if not explicitly caught. The `bug.groovy` file shows the problem, and `bugSolution.groovy` provides a solution.

## Problem
The `methodWithClosure` function executes a provided closure. If the closure throws an exception, the exception is not handled by the `methodWithClosure` function, causing program termination.

## Solution
The solution involves using a `try-catch` block within `methodWithClosure` to handle exceptions thrown by the closure. This ensures that the program continues execution even if an error occurs within the closure.