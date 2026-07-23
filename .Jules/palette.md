## 2026-07-19 - Added global focus visible styles
**Learning:** Found that the main shared stylesheet (`site.css`) lacked `:focus-visible` states, making keyboard navigation difficult across all apps in the portfolio. Adding a global `:focus-visible` ensures consistent, accessible keyboard focus rings without affecting mouse users.
**Action:** Always verify keyboard navigation and focus states early in the audit, as a single CSS rule can significantly improve a11y across an entire site.

## 2026-07-20 - Screen reader noise from decorative icons and skip link focus
**Learning:** Screen readers often announce decorative elements (like emojis in icons or arrow symbols in links), which creates unnecessary noise. Furthermore, skip links (e.g. "Skip to content") need their target container (like `<main id="main">` or `<header id="main">`) to have `tabindex="-1"` so it can receive programmatic focus without interfering with regular tab order.
**Action:** Always add `aria-hidden="true"` to decorative icons/symbols, and ensure the target of a skip link has `tabindex="-1"` to guarantee the focus moves correctly for keyboard users.
