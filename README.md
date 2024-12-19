# Uncommon HTML Bug: Conflicting Style Declarations

This repository demonstrates a subtle bug related to the use of the `display` style property in HTML.  The issue highlights a scenario where sequentially setting the `display` property can lead to unexpected visual results, despite the apparent logic.

The `bug.html` file shows the initial problem. The `bugSolution.html` file provides the fix. 

## Problem Description
The code attempts to initially hide and then show an element using JavaScript. However, setting `display: none;` and then `display: block;` in quick succession doesn't always render the element as expected, potentially leading to an invisible element even after the 'show' command.  This behavior is not always consistent across browsers. 

## Solution
The solution employs a more robust approach to managing element visibility and ensures expected rendering behavior across different browsers.