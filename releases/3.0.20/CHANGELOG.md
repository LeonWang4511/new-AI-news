# 3.0.20 — Control UI craftsmanship and responsive audit

Source: 3.0.19. The main task workspace, Planner conversation, local storage, stage progression, approvals and scene selection are preserved.

### Fixed
- Removed experimental `liquid-glass-material-315` CSS that layered multiple incompatible switch rules.
- Removed `backdrop-filter` from `.glass-control` layout wrapper, the rectangular glass plate visible in the user's mobile zoom video.
- Switch track is a single clipped capsule; thumb vertical offset checked as **0px**.
- Rebuilt icon-only control alignment; SVG geometric centers are **0px offset** in 360px, 390px, 430px, 834px, and 1440px browser samples.
- Added missing `sun` icon definition to the JS icon registry. Before, the icon registry silently used `info` as fallback.
- Corrected mobile back button visibility: hidden in overview, visible in task detail, hidden again after navigating back.
- Increased icon/button hit areas and made the mobile New Task control a simple accessible `+` circle.
- Increased main content gutters, task-row paddings, action spacing; improved text contrast over ambient gradients.
- Simplified layered shadow/gloss so each button gets one visual surface instead of double borders/panels.

### Tested locally (Chromium via injected HTML)
- Responsive viewports: 360x780, 390x844, 430x932, 834x1112, 1440x900.
- Toggle, scene, New Task modal + submit, Planner dialog, Inbox tab, approval action.
- Mobile task-detail drill-in and back navigation.
- No JS uncaught errors or horizontal overflow in tested sizes.
- Checked actual CSS `glass-control` backdrop filter = `none`; switch radius `999px`, overflow `hidden`.

### Known limits
- `backdrop-filter` creates translucent frosted material; this release does not claim the literal optical scene-refraction of Apple Liquid Glass.
- GitHub Pages deploy and device-specific Safari/WebView visual acceptance are not established by the local test alone.