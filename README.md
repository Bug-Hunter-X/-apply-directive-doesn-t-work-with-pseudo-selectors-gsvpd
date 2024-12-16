# Tailwind CSS @apply Directive Bug with Pseudo-selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles when used with pseudo-selectors like `:hover`, `:focus`, or `:active`. This can lead to unexpected behavior in interactive elements.

## Bug Description
The `@apply` directive is intended to apply predefined Tailwind CSS utility classes to a component. However, when this directive is used with classes containing pseudo-selectors, the styles associated with the pseudo-selectors are not applied.

## Reproduction Steps
1. Clone this repository.
2. Open `bug.css` to see the problematic implementation.
3. Open `index.html` (or a similar file in your project) and observe the element that should have the hover effect.
4. You will notice the hover effect does not work as expected.

## Solution
The solution is provided in `bugSolution.css` which demonstrates the correct implementation using direct application of the utility classes without the `@apply` directive for pseudo-selectors. 