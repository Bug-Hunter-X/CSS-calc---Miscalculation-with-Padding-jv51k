# CSS calc() Miscalculation with Padding
This repository demonstrates a common issue encountered when using the `calc()` function in CSS, specifically when dealing with percentages and padding.  The example shows how `calc(100% - 10px)` behaves unexpectedly within a padded container.

## Problem
The `100%` in `calc(100% - 10px)` is calculated based on the content area of the parent element, not including the padding. Thus, the `10px` subtraction is applied to a smaller value than expected, leading to misalignment.

## Solution
The issue can be resolved by either explicitly adding the padding to the calculation or by adjusting the container's `box-sizing` property.