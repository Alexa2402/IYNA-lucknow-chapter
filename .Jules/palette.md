# Palette's Journal

## 2026-11-11 - Accessible Form Controls in Static Landing Pages
**Learning:** In compact static landing page forms that rely on minimalist placeholder-driven styling and custom toggle buttons, screen readers lose critical context: fields lack accessible labels (`<label>` or `aria-label`), button toggles do not announce their selection state without `aria-pressed`, and validation errors inserted dynamically are silent without `aria-live` or `role="alert"`. Furthermore, omitting standard `autocomplete` attributes causes unnecessary typing friction on mobile.
**Action:** Pair every placeholder-only input with a visually hidden `.sr-only` `<label>` tied to its `id`, provide `role="group"` and dynamic `aria-pressed` on multi-choice option buttons, mark dynamic error containers with `role="alert"` and `aria-live="polite"`, and ensure visible `:focus-visible` styling for keyboard navigators.
