# Stopa OS

Stopa OS is the shared visual and interaction language for Zlta Stopa products.

It is not the homepage copied into dashboards. It is the calmer operating layer underneath the same brand: bold type, clean surfaces, precise hierarchy, and restrained accent.

The goal is simple:

- make every product clearly belong to Zlta Stopa
- keep dense data interfaces readable and confident
- preserve room for product-specific ideas
- move fast across different stacks without visual drift

## Positioning

The homepage is expressive and promotional.

Dashboards should feel like a civic data workstation:

- calm
- dense
- sharp
- operational
- trustworthy

The right reference is closer to a beautiful investigative tool than to a generic SaaS admin.

## Core Principles

### 1. Same company, different instruments

Every product should feel related, but not identical.

Shared across products:

- dotted-grid background language
- content width and page gutters
- floating header shell
- radius, border, and shadow system
- typography hierarchy
- search, chips, and action styling
- KPI cards, tables, charts, and detail panels

Allowed to vary per product:

- product name and logo lockup
- one motif or hero move
- one accent family later, once the shell is stable

### 2. Search can own the page

For search-led products like `zmluvy`, search is not a utility tucked into the header. It is the primary move.

That means:

- search sits below the header, not crammed into it
- the search stage gets air through surrounding space, not a giant input
- one short supporting line is enough
- filters can stay visible as a horizontal chip row

### 3. Calm and dense

The interface should show a lot without feeling crowded.

That means:

- more air between major sections than inside components
- compact controls
- compact KPI cards
- full-width primary data surfaces when the content wants room
- fewer decorative elements doing more work

### 4. Flat over plastic

Stopa OS should feel tactile, not glossy.

Use:

- subtle background shifts
- soft borders
- restrained shadows
- clear focus states

Avoid:

- glossy gradients on controls
- candy-like search fields
- deep ornamental shadows
- decorative chrome competing with data

### 5. Accent is a scalpel

Yellow is not wallpaper.

Use accent for:

- active tabs and chips
- primary actions
- focus states
- one highlighted KPI or callout
- selected rows or important states

Do not spread accent across every surface on the page.

### 6. Portable implementation

The source of truth must work across static HTML, React, server-rendered pages, and future stacks.

That means:

- tokens in JSON
- tokens in CSS variables
- reusable HTML/CSS patterns
- previews that demonstrate intent

## Shared Visual Language

### Background

The suite background is a neutral dotted grid.

Rules:

- dots are neutral, not yellow
- the grid stays quiet behind content
- content surfaces float above it
- the grid can fade under denser regions

This is a suite-level signature, not a hero effect.

### Header

The top bar is a floating control strip and should remain visible while working.

Rules:

- compact enough to avoid eating the fold
- elevated enough to read as a distinct shell
- real logo allowed, but not oversized
- do not put an extra border around the full logo
- pair the logo with one short human claim above the product name
- avoid repeating the suite name and product name in stacked labels
- core destinations like `Prehľad`, `Zoznam`, `Metodika`, or `Datasette` belong in primary nav
- reserve the right side for utility actions such as search jump or issue reporting
- issue-report actions may use a thick accent outline in their default state
- a search-jump icon in the header is fine
- page search still lives below the header

### Search Stage

The default search-first pattern is:

1. floating top bar
2. one short claim
3. one centered search field
4. visible horizontal chip row
5. supporting text only if it helps

Rules:

- use one short functional kicker above the field, not a separate centered slogan plus another label
- search field should feel easy to hit, not monumental
- the main page search may sit on a brighter white surface than surrounding controls so it reads as the primary instrument
- aim for roughly `48-56px` desktop search height
- the entire search shell should be clickable and focus the input
- focus should visibly shift the field background, not only add a ring
- search action should sit flush to the far right edge of the field
- keyboard hint should use an OS-style keycap, for example `Stlac / pre vyhladavanie`
- a quick-filter label may sit inline to the left of the chips
- avoid helper text that only repeats the placeholder
- placeholder text should be short and concrete

### Surfaces

Surfaces should be bright, warm, and lightly elevated.

Rules:

- mostly white or near-white cards
- soft graphite border
- subtle shadow
- flatter controls than cards
- nested surfaces should differ through tone, not color overload
- scrollable panels may use a quiet amber scrollbar on a warm track

### Typography

Typography should feel editorial, but efficient.

Recommended families:

- display: `Public Sans`
- UI: `Inter`
- mono: `IBM Plex Mono`

Rules:

- titles are bold and direct
- KPI numerals are heavy and fast to scan
- labels are quiet and uppercase only when useful
- body copy should stay short

### Shape

Roundedness should feel deliberate, not bubbly.

Rules:

- slightly tighter radii than the homepage
- compact pills and chips
- strong shell radius for the floating header
- medium radius for cards, search, and table shells

### Depth

Depth should separate layers, not decorate them.

Rules:

- one soft card shadow
- slightly stronger floating-header shadow
- minimal hover lift
- no stacked glow effects in dense views

## Layout Rules

### Width

Use a shared max content width and consistent side gutters.

Side breathing room matters. Pages should not feel edge-to-edge unless a deliberate data view truly needs it.

### Rhythm

Use one spacing scale everywhere.

The important rule is:

- major sections breathe
- components stay compact

### Page Anatomy

Default search-first dashboard anatomy:

1. floating top bar
2. search stage
3. KPI row
4. primary data surface
5. secondary charts, details, or notes

Default list-first or detail-first pages can compress the search stage, but should keep the same shell language.

## Component Rules

### KPI Cards

KPI cards should be compact and mostly neutral.

Rules:

- standard KPI cards stay plain
- at most one KPI in a row should use a stronger accent treatment by default
- search-first overview pages should prefer six KPIs on desktop, typically a clean `3 x 2`
- drop the weakest metric rather than forcing an awkward seventh card
- prefer a subtle top accent for the highlighted KPI
- do not use the full vertical rail on every KPI

### Accent Rail

The vertical accent rail is still part of the system, but it is reserved.

Use it for:

- callouts
- selected records
- warnings
- narrative summaries

Do not use it as the default treatment for ordinary metrics.

### Tables

Tables should feel like the main instrument, not leftover admin UI.

Rules:

- primary lists can take full width inside the page frame
- sticky headers when useful
- subdued separators
- selected row uses accent inset or rail
- hover should be a soft tint, not a loud fill

### Filters

Filters should feel fast and visible.

Rules:

- visible horizontal chip row is the default
- active state should be obvious
- reserve collapsible filter panels for advanced controls

### Charts And Details

Charts and detail cards should reuse the same shell language as tables and KPI cards.

Rules:

- neutral wrappers
- restrained grid lines
- one accent color per chart unless the comparison truly needs more
- ranking charts should stay mostly monochrome, with highlight used sparingly
- categorical charts should aggregate the long tail into `Ostatné` when the legend gets noisy
- avoid rainbow palettes or more than roughly `6-8` clearly distinct category colors in one view
- detail pages should explicitly label enriched or extracted titles versus the original source title
- yellow-trace or signal surfaces should use amber signal styling, not destructive red, unless the state is truly an error
- external suite links should use a proper icon treatment instead of a raw text arrow
- details should not visually overpower the primary list

## Color Strategy

For now, the suite stays on one shared yellow accent.

That is deliberate.

It keeps the shell coherent while the first redesigns settle. Product-specific accent families can come later, once `zmluvy` and `majetkovy-kompas` clearly feel like the same system.

Keep these color layers separate:

- suite brand accent
- future product accent
- semantic colors

Semantic colors must mean the same thing everywhere.

## What Ships In The System

Stopa OS should stay practical.

Ship:

- `DESIGN.md`
- `tokens.json`
- `tokens.css`
- `patterns/patterns.css`
- HTML pattern snippets
- preview pages

This is enough to keep humans and AI aligned without forcing every product into the same framework.
