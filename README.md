# CSS Specificity Conflict Bug

This repository demonstrates a common CSS bug related to specificity conflicts.  The bug occurs because of unexpected style overriding due to the higher specificity of a class selector over an element selector.

## Bug Description

The `bug.css` file contains CSS code with conflicting styles for a `<p>` element inside a container class.  The class selector `.highlight` has higher specificity and overrides the style defined for the `p` element, resulting in unexpected styling.

## Solution

The `bugSolution.css` file provides a solution to this problem. One solution is to use the `!important` flag to increase the specificity of the `p` selector, although this should be used sparingly.  A better approach is to refactor the CSS for better specificity management and to resolve the conflicting styles by making sure the more specific selector is the one applied when both selectors are applied to the same element.  Another solution would be to use more specific selectors to avoid the conflict altogether. 