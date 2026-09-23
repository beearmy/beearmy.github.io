## 2026-07-19 - Added global focus visible styles
**Learning:** Found that the main shared stylesheet (`site.css`) lacked `:focus-visible` states, making keyboard navigation difficult across all apps in the portfolio. Adding a global `:focus-visible` ensures consistent, accessible keyboard focus rings without affecting mouse users.
**Action:** Always verify keyboard navigation and focus states early in the audit, as a single CSS rule can significantly improve a11y across an entire site.

## 2026-09-23 - Skip link target focus
**Learning:** Found that skip link targets must use `tabindex="-1"` for correct programmatic focus, otherwise screen readers and keyboard navigation may not work properly across all browsers (specifically WebKit/Safari). Also noticed Rep Bank pages were missing skip links entirely.
**Action:** Always ensure skip-to-content links exist on all pages and that their corresponding `#main` target elements have `tabindex="-1"` to properly handle programmatic focus without interfering with natural tab order.
