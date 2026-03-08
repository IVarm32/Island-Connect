## 2025-05-22 - Restoring Standard Affordances
**Learning:** Forcing `cursor: default` on interactive elements (`<a>`, `<button>`) breaks user expectations and makes the UI feel unresponsive. This pattern was prevalent throughout the initial codebase.
**Action:** Always ensure interactive elements use the standard pointer cursor and avoid inline `style="cursor: default;"` on links.

## 2025-05-22 - Static Tailwind Verification
**Learning:** This repository is a static site with a pre-compiled `style.css`. Adding new Tailwind utility classes to `index.html` will fail to render unless the class already exists in the CSS bundle.
**Action:** Before applying Tailwind classes in a static repo, verify their presence in `style.css` using `grep`.
