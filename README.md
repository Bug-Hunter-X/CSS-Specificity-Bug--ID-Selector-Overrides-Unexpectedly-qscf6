# CSS Specificity Bug: ID Selector Overrides Unexpectedly

This repository demonstrates an uncommon bug related to CSS specificity. The bug involves unexpected behavior when combining ID and class selectors due to the higher specificity of ID selectors.

## Bug Description
The unexpected overriding of styles occurs because the ID selector (`#myElement`) has a higher specificity than the class selector (`.myClass`), even if `.myClass` appears later or there is a more specific rule that includes both selectors.

## How to Reproduce
1. Clone this repository.
2. Open `bug.css` and observe the CSS rules.
3. Create an HTML file with an element having both the ID `myElement` and the class `myClass`.
4. Link the CSS file to the HTML.
5. Observe that the text color is red instead of green, despite `#myElement.myClass` being declared last.

## Solution
The solution involves understanding and adjusting the CSS specificity rules. The solution is given in `bugSolution.css`.