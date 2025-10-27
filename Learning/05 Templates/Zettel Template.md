---
id: <% tp.date.now("YYYYMMDD-HHmm") %>
title: <% tp.file.title %>
type: Zettel
tags:
  - Zettel
  - #Math / #CS / #Physics / #Finance
area:
created: <% tp.date.now("YYYY-MM-DD") %>
updated: <% tp.date.now("YYYY-MM-DD") %>
formulas: []
code_examples: []
diagrams: []
---
# <% tp.file.title %>


## Summary / Definition
- 

## Deep Explanation
- 

## Formulas / Equations
- Inline: $E = mc^2$
- Block:
$$
\iiint_V f(x,y,z) \, dx\,dy\,dz
$$

## Code / Algorithm Example
```python
# Example code
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)