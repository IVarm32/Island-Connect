## 2025-03-09 - [Anti-pattern: cursor: default on interactive elements]
**Learning:** This app extensively used `style="cursor: default;"` on anchor tags and buttons, which breaks standard browser affordances and confuses users about what is interactive.
**Action:** Always check for and remove manual cursor styles on links and buttons to ensure the standard pointer cursor is displayed.

## 2025-03-09 - [Accessibility: Missing form label associations]
**Learning:** Form inputs and textareas in the "Service Request" section lacked `id` attributes, preventing explicit association with their `<label>` elements via the `for` attribute.
**Action:** Ensure all form controls have unique `id`s and matching `for` attributes on their labels to support assistive technologies.
