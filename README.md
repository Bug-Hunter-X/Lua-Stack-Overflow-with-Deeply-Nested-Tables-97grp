# Lua Stack Overflow with Deeply Nested Tables

This repository demonstrates a common Lua error: a stack overflow caused by deeply nested tables when using recursive traversal. The issue arises when the recursion depth exceeds the Lua interpreter's stack limit.

## Bug Description
The provided Lua code recursively iterates through a nested table using `pairs`.  While functional for shallowly nested tables, this approach fails for deeply nested structures, resulting in a stack overflow error.

## Solution
The solution involves implementing iterative traversal to avoid excessive recursion depth. This prevents stack overflow errors, even with extremely deep nesting.