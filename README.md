# F# Mutability Gotcha: Unexpected Behavior with Mutable Variables

This example demonstrates a potential issue with mutable variables in F#. When a function uses mutable variables, subsequent modifications to those variables outside the function's scope might not affect the function's behavior as expected.

## Bug Description
The `add` function calculates the sum of `x` and `y`. However, changing the values of `x` and `y` after calling `add` doesn't update the result.

## Solution
The solution involves recalculating `z` after modifying `x` and `y` or using a different approach that doesn't rely on mutable variables.