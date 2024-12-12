# Subtle Type Handling Issue in Hack Function Calls

This repository demonstrates a subtle type-handling issue that can occur in Hack when dealing with function calls and type annotations.  The problem is not a straightforward type mismatch, but rather a less common scenario that can lead to unexpected behavior or compiler errors depending on the specific Hack version and compiler settings.

The `bug.hack` file contains the problematic code. The `bugSolution.hack` file offers a solution, demonstrating how to correctly handle the situation.

## Problem Description

The code in `bug.hack` defines two simple functions: `foo` and `bar`.  Both functions have clear type annotations. However, a subtle issue exists in the way `bar` calls `foo`. The compiler might not immediately flag this as an error, depending on the compiler's type inference and checking mechanisms.