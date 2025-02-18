# Handling JSON Decoding Errors in Dart

This example showcases a potential issue when working with JSON in Dart and how to handle it gracefully.

## The Problem

The `fetchData` function fetches data from a remote API.  If the API returns invalid JSON, the `jsonDecode` function will throw a `FormatException`. The original code lacks proper handling for this exception, leading to potential crashes.

## The Solution

The solution involves wrapping the `jsonDecode` call in a `try-catch` block to specifically catch `FormatException`. This allows the application to handle the error gracefully instead of crashing.

## How to Use

1.  Clone this repository.
2.  Run the `bug.dart` file to see the original error.
3.  Run the `bugSolution.dart` file to see the corrected code.
