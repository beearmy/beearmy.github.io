## 2026-07-19 - Added global focus visible styles
**Learning:** Found that the main shared stylesheet (`site.css`) lacked `:focus-visible` states, making keyboard navigation difficult across all apps in the portfolio. Adding a global `:focus-visible` ensures consistent, accessible keyboard focus rings without affecting mouse users.
**Action:** Always verify keyboard navigation and focus states early in the audit, as a single CSS rule can significantly improve a11y across an entire site.
