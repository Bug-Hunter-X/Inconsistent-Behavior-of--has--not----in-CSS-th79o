# Inconsistent Behavior of :has(:not()) in CSS

This repository demonstrates an uncommon bug related to the interaction between the `:has()` and `:not()` pseudo-classes in CSS.  The issue lies in the inconsistent behavior observed across different browsers when using `:has(:not())` to target elements based on the absence of specific child elements.

The `bug.css` file contains the problematic CSS code, and `solution.css` illustrates a potential workaround using a different approach to achieve the desired styling.

## Problem

The primary issue is that the selector `:has(:not(.item))` doesn't reliably identify containers that lack `.item` children in all browsers. This leads to unexpected styling.

## Solution

The solution file, `solution.css`, provides an alternative approach to achieve the same styling effect with more consistent browser support. The proposed solution leverages the `:empty` pseudo-class which is more reliably supported across all browsers, therefore leading to more predictable results.
