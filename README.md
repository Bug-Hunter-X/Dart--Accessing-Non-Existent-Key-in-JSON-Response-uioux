# Dart: Handling Non-Existent Keys in JSON Responses

This repository demonstrates a common error in Dart when working with JSON responses: attempting to access a key that does not exist in the JSON data.  The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides a corrected version.

## Problem

The original code attempts to access a key ('nonExistentKey') that may not always be present in the JSON response from the API. This leads to a runtime error if the key is missing.

## Solution

The solution involves checking for the existence of the key before attempting to access its value. This prevents runtime exceptions and makes the code more robust.  The solution uses the `containsKey` method to check for the key's presence.