# RootFrond Team Guide

## Shared ownership rules
To reduce Git merge conflicts, one person should own `index.html` integration. Other team members can develop their section in separate files/branches, then the integration owner pastes each section into the matching placeholder.

### Suggested section ownership
- `overview` — project overview and problem summary
- `how-it-works` — workflow / how the system works
- `disease-detection` — RootFrond NPK sensor + leaf-image analysis feature (legacy ID kept)
- `farmer-stories` — hypothetical farmer scenarios / validated findings when available
- `team` — team profiles and responsibilities
- `early-access` — project interest form / pilot information

## What each member should send to the integration owner
1. One `<section id="...">...</section>` block only.
2. CSS with section-specific class names, for example `.overview-hero` or `.team-card`.
3. Any image assets and their relative paths.
4. A short note about any JavaScript the section requires.

## Navigation rule
The navigation link and section ID must match exactly:
- `href="#overview"` → `id="overview"`
- `href="#how-it-works"` → `id="how-it-works"`
- `href="#disease-detection"` → `id="disease-detection"`
- `href="#farmer-stories"` → `id="farmer-stories"`
- `href="#team"` → `id="team"`
- `href="#early-access"` → `id="early-access"`

## Before merging
- [ ] Check the console for errors.
- [ ] Test mobile menu and dark mode.
- [ ] Check for horizontal scrolling at 320px width.
- [ ] Check that every navigation/footer anchor reaches an existing ID.
- [ ] Confirm images have descriptive `alt` text.
- [ ] Confirm claims and statistics are sourced; hypothetical scenarios are not represented as interview quotes.


## RootFrond section ownership — preserved
- Anupama: `overview` and `faq` (HTML, Anupama CSS, Anupama JS).
- Janith: `how-it-works` (HTML, Janith CSS, Janith JS flow).
- Janani: `disease-detection` (ID deliberately kept; displayed as Nutrient Analysis).
- Sudil: `farmer-stories` (ID deliberately kept; displayed as Farmer Insights).
- Isindu: `team`, `early-access`, and app-preview content.

Keep each member's `SECTION START/END`, `Styles`, and `Script` comments intact.
