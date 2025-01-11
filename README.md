# Uninitialized Property Access in C#

This repository demonstrates a common C# error: a `NullReferenceException` caused by accessing an uninitialized property.

The `bug.cs` file shows the problematic code.  The `bugSolution.cs` file provides a corrected version.

## Problem

In C#, class properties default to `null` (or their type's default value) unless explicitly initialized. Accessing a property before assigning a value results in a `NullReferenceException`.

## Solution

Always initialize properties, either in the constructor or before use. Consider using nullable types to indicate the possibility of null values and handle them appropriately using null-conditional operators or null checks.