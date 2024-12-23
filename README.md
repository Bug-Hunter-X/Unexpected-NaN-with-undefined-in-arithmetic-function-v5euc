# Unexpected NaN with undefined in arithmetic function

This repository demonstrates a common JavaScript error involving the handling of `undefined` values in arithmetic operations.  The original code lacks a check for `undefined`, resulting in `NaN` outputs when an `undefined` value is encountered. The solution provides a comprehensive check for both `null` and `undefined` values.

## Bug
The bug lies in the `foo` function's handling of input values. The function correctly handles `null` values by returning `null`, however, it does not handle `undefined` values correctly. This leads to unexpected `NaN` (Not a Number) results when an `undefined` value is used in the addition operation.

## Solution
The solution modifies the `foo` function to check for both `null` and `undefined` values, returning `null` in those cases. This prevents the generation of `NaN`, ensuring more predictable function behavior.