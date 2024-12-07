# Inconsistent calc() function behavior with dynamic parent widths

This repository demonstrates a CSS bug related to the `calc()` function and dynamically sized parent elements.

## Bug Description
The provided CSS snippet utilizes `calc()` to determine the width of a `div` element, subtracting a padding value from 100% of its parent's width. However, inconsistent rendering is observed across different browsers when the parent's width is not explicitly set and is instead determined dynamically (e.g., by the content).

## Solution
The issue is addressed by setting an explicit width for the parent container or by using a different approach for calculating the width of the child element, like using viewport units or flexbox.