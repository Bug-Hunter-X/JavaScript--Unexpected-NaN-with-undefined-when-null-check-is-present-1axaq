# JavaScript Unexpected NaN Bug

This repository demonstrates a common JavaScript error involving unexpected NaN results when using loose comparisons and handling undefined values.

## Bug Description

The `foo` function intends to return 0 if the input `x` is `null`. However, if `x` is `undefined`, it incorrectly produces `NaN`. This happens because `undefined + 1` evaluates to `NaN`.

## Solution

The solution involves explicitly checking for both `null` and `undefined` before performing the addition. This ensures that the function always returns a valid number in the intended scenarios.
