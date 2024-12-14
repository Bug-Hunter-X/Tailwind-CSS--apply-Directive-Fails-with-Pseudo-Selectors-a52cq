# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles correctly when used with pseudo-selectors such as `:hover`, `:focus`, or `:active`. The issue is particularly noticeable when combined with responsive design directives.

## Bug Description

The `@apply` directive doesn't correctly handle the cascading of styles for pseudo-selectors, resulting in these styles not being applied as expected. This can lead to unexpected behavior and inconsistencies in the user interface.

## Reproduction

1. Clone this repository.
2. Open `index.html` in a web browser.
3. Observe that the hover effect is not applied to the button.

## Solution

The recommended approach is to avoid using `@apply` with pseudo-selectors. Instead, directly apply the styles within your components or use the `@layer` directive for more robust style management. The solution file provides an updated version of the CSS to demonstrate this.