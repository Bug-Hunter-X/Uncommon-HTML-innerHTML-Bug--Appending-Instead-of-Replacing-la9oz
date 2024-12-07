# Uncommon HTML innerHTML Bug

This repository demonstrates an uncommon bug related to the usage of `innerHTML` in HTML.  The bug arises from a misunderstanding of how `innerHTML` behaves when combined with string concatenation and existing content within the target element.

## Bug Description
The code attempts to replace the content of a div element using `innerHTML`. However, due to the concatenation of the new content with the existing `innerHTML`, the new content is appended instead of replacing the original content. This is an unusual behaviour and might not be immediately apparent to developers unfamiliar with the nuances of `innerHTML`.

## Solution
The solution involves replacing the existing `innerHTML` completely with the new content, avoiding concatenation.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the new text is appended to the existing text instead of replacing it.
4. Open `bugSolution.html` to see the corrected version.