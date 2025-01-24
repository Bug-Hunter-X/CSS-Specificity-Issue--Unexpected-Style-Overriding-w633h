# CSS Specificity Bug

This repository demonstrates a common CSS issue related to specificity. The `bug.css` file contains CSS code where styles intended for a class are unexpectedly overridden by a more specific selector. The `bugSolution.css` file provides a solution to this problem.

## Bug

The main issue is caused by the selector `#myId .container`. Because ID selectors have higher specificity than class selectors, styles applied to `#myId .container` will override styles applied to `.container` even if the `.container` styles are defined later in the CSS file.

## Solution

The solution involves either increasing the specificity of the `.container` styles to match or exceed that of `#myId .container`, or restructuring the CSS to avoid the conflict entirely. The `bugSolution.css` file showcases one approach to solving this problem.