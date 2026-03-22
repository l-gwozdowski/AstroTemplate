# Accessibility Audit Notes (WCAG 2.2 AA Baseline)

Generated on: 2026-03-22

## Implemented in the template

- Skip link to main content (`#main-content`).
- Keyboard-operable mobile navigation and header controls.
- Visible `:focus-visible` outline for interactive elements.
- Separate `Light/Dark` toggle button.
- Separate `High Contrast` toggle button, always available in both theme modes.
- High contrast mode consistently uses black background with yellow accent.
- Theme toggle is intentionally disabled while high contrast mode is active.
- Font size controls (`A-`, `A+`) with two persisted sizes: `100%` and `130%`.
- Preference persistence in `localStorage` for theme, contrast, and font size.
- Respect for system settings: `prefers-color-scheme` and `prefers-contrast`.
- Blog post navigation enhancements: back to blog, previous post, next post.

## Automated checks executed

- `npm run astro -- check`
Result: `0 errors`, `0 warnings`, `0 hints`.
- `npm run build`
Result: successful static build.

## Manual WCAG checklist status

- [x] Keyboard focus is visible.
- [x] Keyboard access for all header controls.
- [x] Skip-link implemented and focusable.
- [x] User can increase and decrease text size from UI.
- [x] User can enable high contrast mode from UI.
- [x] Theme and contrast preferences persist between sessions.
- [ ] Screen-reader regression tests on target stack (NVDA/JAWS/VoiceOver) still required.
- [ ] Contrast ratio verification for final real content (copy, images, brand palette) still required.
- [ ] Form-specific accessibility checks still required if forms are added.

## Recommended manual verification flow

1. Test keyboard-only navigation across all pages.
2. Test with at least one Windows screen reader and VoiceOver on macOS.
3. Validate contrast ratios for production copy and media.
4. Re-run checks after each major visual/content change.
