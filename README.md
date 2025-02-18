# Unhandled FormatException in JSON Decoding in Dart

This repository demonstrates a common error in Dart when dealing with JSON responses from network requests: not explicitly handling `FormatException` that can occur during `jsonDecode`. The `bug.dart` file showcases the error, while `bugSolution.dart` provides a corrected version.

## Problem
The original code fails to handle `FormatException` that can be thrown by `jsonDecode` if the response body isn't valid JSON.  This can lead to crashes or unexpected behavior.

## Solution
The solution improves the error handling by using a `try-catch` block specifically to catch `FormatException`. This allows for more graceful handling of invalid JSON responses.