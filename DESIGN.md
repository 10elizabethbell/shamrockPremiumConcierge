---
name: Shamrock Transportation
description: One-man NJ <-> Florida driveaway service, premium concierge. A night highway on deep Irish green, with ivory stationery sections.
colors:
  ground-deepest: "#0d2b21"
  ground-night: "#11352a"
  ground-journey: "#174233"
  ground-glass: "#24573f"
  leaf: "#46a96a"
  ivory: "#f5efe2"
  paper: "#fbf8f1"
  ink: "#173a2d"
  ink-soft: "#4a5f55"
  cream: "#efe7d4"
  cream-soft: "#d3dcbd"
  gold: "#c9a96a"
  gold-deep: "#8a6728"
  taillight: "#d9573f"
  rule-dark: "rgba(201,169,106,.35)"
  rule-light: "rgba(138,103,40,.32)"
  error: "#a3342a"
typography:
  display:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(58px, 17vw, 112px)"
    fontWeight: 600
    lineHeight: 0.92
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(44px, 12vw, 76px)"
    fontWeight: 600
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(32px, 8vw, 42px)"
    fontWeight: 600
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  list-item:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(27px, 7vw, 34px)"
    fontWeight: 600
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, system-ui, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(19px, 4.9vw, 22px)"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, system-ui, Helvetica Neue, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.6
  button:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, system-ui, Helvetica Neue, Arial, sans-serif"
    fontSize: "19px"
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: "0.01em"
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, system-ui, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.12em"
rounded:
  focus: "4px"
  stationery: "6px"
  call: "10px"
  field: "12px"
  form: "22px"
  pill: "999px"
spacing:
  gutter-narrow: "16px"
  gutter: "20px"
  gutter-wide: "40px"
  section: "64px"
  section-wide: "104px"
  column-gap: "64px"
  wrap: "1160px"
components:
  button-gold:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ground-deepest}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "60px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "60px"
  button-green:
    backgroundColor: "{colors.ground-journey}"
    textColor: "{colors.cream}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "60px"
  rates-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.stationery}"
    padding: "38px 28px 32px"
  estimate-form:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.form}"
    padding: "28px 22px 26px"
  input:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "56px"
---

# Design System: Shamrock Transportation

## Overview

**Creative North Star: "The Night Drive, Long Exposure"**

A night highway seen from above, photographed on a long exposure: gold headlight trails one way, red taillights the other, and Ed's car in the middle. Everything else on the page is the hotel stationery you'd find in the glovebox of that drive: ivory paper, thin gold rules, a serif that looks engraved. The pace is calm and unhurried; nothing pops, things drift.

The page alternates two grounds, deep green night and ivory paper, joined by wavy lane-line seams. Structure comes from rules and type, not from boxes: lists are ruled, sections are full-bleed, and only two objects on the whole page are cards (the rates stationery and the estimate form). Type is big for a 60+ reader on a phone: body never under 17px, primary actions 60px tall.

Motion belongs to the road. The hero canvas, the lane seams and the step car are the only moving things, and every one of them stops for reduced motion and when off screen.

**Key Characteristics:**
- Deep Irish green ground, never black; ivory and paper for reading sections.
- Cormorant display with one gold italic turn of phrase per heading; system sans for everything read or tapped.
- Thin gold rules and dashed gold lane markings as the only ornament.
- Pill buttons, gold on green, green on ivory; hover and focus share one outline ring.
- Taillight red lives only inside the motion (canvas, still-frame trails).

## Colors

A two-ground palette (green night, ivory day) with one metallic accent that shifts tone to stay legible on each ground.

### Primary
- **Muted Lounge Gold** (gold): trim on green. Hero italic line, trust titles, the big phone number, footer motto, lane-line dashes, step-rail progress, the primary Call button fill, text selection.
- **Antique Gold** (gold-deep): the same gold, darkened to read on ivory. Italic accents in ivory headings, hover/focus ring on ivory, input focus border, caret, FAQ icon hover.

### Secondary
- **Shamrock Leaf** (leaf): the shamrock mark only (wordmark and favicon) and a faint radial glow in the hero sky (16% alpha). Not a UI color.

### Tertiary
- **Taillight Red** (taillight): canvas and the pre-JS still-frame trail only. The car's trail ribbon, oncoming streaks. Never on text, buttons or borders.

### Neutral
- **Night Green** (ground-night): body and hero ground, `on-dark` sections, theme-color.
- **Journey Green** (ground-journey): "How it works" and trust sections; green button fill on ivory.
- **Deepest Green** (ground-deepest): footer ground, text on the gold button, shadow tint.
- **Glass Green** (ground-glass): car windows (step car SVG and canvas car).
- **Ivory** (ivory): paper sections (`on-light`).
- **Paper** (paper): the two cards that sit on top of a ground (rates, estimate form). Always one step lighter than what it sits on.
- **Ink / Ink Soft** (ink, ink-soft): headings and secondary copy on ivory/paper.
- **Cream / Cream Soft** (cream, cream-soft): headings and secondary copy on green.
- **Rule Dark / Rule Light** (rule-dark, rule-light): 1px gold hairlines; dark on green, light on ivory.
- **Error Brick** (error): field error border and message. Hardcoded in CSS, not yet on `:root`; promote it if more states appear.

### Named Rules
**The Never-Black Rule.** The darkest value on the page is ground-deepest. No `#000`, no neutral greys; shadows are tinted from the ground green. The canvas car and the step car's drop shadow use black at 35-45% alpha; that is illustration paint, not a precedent for UI shadows.

**The Ground-Matched Gold Rule.** On green, use gold; on ivory or paper, use gold-deep. Same for rules (rule-dark vs rule-light) and text (cream vs ink). Every element picks its pair from the ground it sits on, never across.

**The Red-Stays-On-The-Road Rule.** Taillight red appears only inside moving imagery. It is not an accent color.

## Typography

**Display Font:** Cormorant (Cormorant Garamond, self-hosted latin subset in `fonts/`, weights 500-700 roman and italic) with Iowan Old Style / Palatino / Georgia fallback.
**Body Font:** system sans stack (-apple-system, Segoe UI, system-ui).

**Character:** an engraved, high-contrast serif for everything said, a plain native sans for everything read at length or tapped. The serif is big and tight; the sans is big and loose.

### Hierarchy
- **Display**: hero h1 only. Steps to a fixed 128px at 1100px+. Second line is italic 500 in gold, set on its own line.
- **Headline**: section h2. "Pack it full" is the deliberate exception at `clamp(56px, 15vw, 104px)`, the second-biggest type on the page; the rates card h2 drops to `clamp(40px, 10.5vw, 60px)`.
- **Title**: h3 in steps, trust, form (range 30-46px depending on context).
- **List item**: ruled serif rows (pack 500, where 600, FAQ summary 600 at `clamp(24px, 6.2vw, 30px)` / 1.22).
- **Phone number**: serif 600 `clamp(42px, 12vw, 72px)`, lining tabular figures, gold. The number is set as type, not as a button.
- **Lede**: one sentence under an h2, max 34ch, soft color.
- **Body**: 18px / 1.6 (19px from 760px). Measure 30-40ch in sections, 62ch in FAQ answers.
- **Label**: uppercase tracked sans, 12.5-15px, 0.12-0.2em. Only for the wordmark's "Transportation", the top-bar route, and the right-hand tags in the pack list.

### Named Rules
**The One Italic Rule.** Each heading may turn one phrase italic 500, colored gold (green ground) or gold-deep (ivory). That phrase carries the meaning ("I'll drive.", "full.", "Very reasonable rates."). Never italicize a whole paragraph.

**The 17px Floor.** Nothing the customer reads drops below 17px (16px only for the copyright line). Labels are the one smaller register, and they are never sentences.

**Tight Serif, Loose Sans.** Serif headings sit at 0.92-1.22 line height; sans copy at 1.5-1.6. The tight leading on display is intentional.

## Layout

Single-scroll, phone-first one-pager. Content sits in a centered wrap (max 1160px) with a side gutter of 20px (16px under 370px, 40px from 760px). Sections are full-bleed grounds with vertical padding of 64/72px on phones and 104/112px from 760px.

**Breakpoints** (min-width unless noted):
- **base (phone)**: everything stacks; hero buttons stack full-width (max 420px); the road sits below the hero copy and fills the rest of the first screen (min 230px).
- **max 370px**: narrower gutter, smaller button text and padding, smaller wordmark.
- **760px**: gutter 40px, body 19px, top-bar route appears, hero buttons sit side by side, the road goes full-bleed behind the hero copy, trust list goes 3 columns, journey becomes a 2-column grid with a sticky h2, footer 3 columns. Lane seams 44 to 60px tall.
- **960px**: pack, where/rates, estimate and FAQ go two-column (64px gap); FAQ h2 becomes sticky.
- **1100px**: hero h1 fixed at 128px; form fields pair up two per row.

**The Ruled List Rule.** Lists of facts (pack, where, trust, FAQ) are rows separated by 1px rules, top rule on the first item, no bullets, no boxes. Row padding 16-24px vertical. On desktop the trust list turns into three columns each topped by one rule.

**The Sticky Headline Rule.** In two-column sections where the right column is long (journey, FAQ), the h2 sticks at 96px from the top.

## Elevation & Depth

Mostly flat: depth comes from the two-ground alternation and from the paper cards sitting one step lighter than their ground. Shadows are soft, long, negatively spread and tinted green (never neutral black).

### Shadow Vocabulary
- **Soft** (`--shadow-soft`: `0 14px 28px -16px rgba(0,0,0,.28), 0 3px 8px -4px rgba(0,0,0,.12)`): green button.
- **Gold lift** (`0 14px 30px -14px rgba(6,26,19,.55)`): gold button on green.
- **Form float** (`0 30px 60px -30px rgba(6,26,19,.6)`): estimate form on green.
- **Car drop** (`drop-shadow(0 6px 8px rgba(0,0,0,.35))`): the step car only, so it reads above the rail.

**The Lit-From-Above Rule.** Every shadow falls straight down with a negative spread, so it reads as ambient light under an object, never a hard offset or a glow halo.

## Shapes

Round where you touch, square-ish where you read. Buttons are full pills (999px); the direction contract said "no pills", but the build ships pill buttons throughout and they are recorded here as the system (no pill-shaped chips or tags exist). Inputs are gently rounded (12px), the estimate form generously (22px). The rates card is near-square (6px), drawn as stationery: a 1px rule-light border plus a second 1px rule inset 9px (outline with negative offset), the double-ruled border of a hotel card. Focus rings round to 4px. Dividers are never straight lines between grounds: see Lane-line dividers.

## Components

### Buttons
- **Shape:** full pill (999px), 60px min height, 26px side padding, 21px leading SVG icon, 1.5px border.
- **Gold:** the primary Call action on green. Phone number inside in tabular figures at 85% opacity.
- **Ghost:** transparent with a 55% cream border, cream text; the secondary action on green.
- **Green:** journey-green fill, cream text, soft shadow; the action on ivory/paper (rates card, form submit).
- **Hover / Focus:** a 2px outline ring at 3px offset in the ground's ring color (cream on green, gold-deep on ivory), plus a 1px lift; press drops 1px. Transform and shadow ease over 0.5s on `cubic-bezier(.16,1,.3,1)`.
- One call to action per block; the hero has exactly two (gold, ghost).

**The One Ring Rule.** Hover and keyboard focus look the same: a 2px outline at 3px offset. Sections set `--ring` (`on-dark`: cream; `on-light` and the form: gold-deep) and every interactive thing (buttons, big number, FAQ summaries, footer and form links, inputs) uses it. Don't introduce color-fill hovers.

### Lane-line dividers (signature)
A 44px (60px from 760px) SVG seam between every pair of sections. The upper ground fills the background, the lower ground fills a gently waving path, and a gold dashed line (3px, dash 26/18, round caps) runs 11px inside the lower color like a road marking. The wave and dashes drift slowly (amplitude 7px, dash 8px/s). Set `data-from` / `data-to` to the two grounds' hexes. Every section boundary uses one; never a straight edge or an `<hr>`.

### Ruled lists
Pack (serif rows, uppercase tag right-aligned), Where (serif rows with a sans `small` line under), Trust (gold serif title plus cream-soft line), FAQ (`details` rows: serif summary, 64px min height, thin plus icon rotating 45 degrees on open, height animates via `::details-content`).

### Rates card (stationery)
Paper on ivory, double gold hairline border, 6px radius, padding 38/28/32 (48/44/44 from 760px). Headline in gold-deep italic, one paragraph, one green button. The real rates table, once Ed confirms, goes in this card in the same style.

### Estimate form
Paper card on green, 22px radius, form-float shadow, sets `--ring: gold-deep`. Labels 18px 600 ink above fields; "(optional)" set in normal-weight ink-soft. Inputs white, 1.5px ink-at-28% border, 12px radius, 56px min height; hover and focus switch border and outline to gold-deep. Errors: brick border plus a 17px brick message under the field, linked with `aria-describedby`. Submit is a full-width green button. It composes an SMS, not a server post.

### Navigation
No nav menu. The top bar is the shamrock wordmark (leaf-green mark, cream serif "Shamrock", gold tracked "Transportation") and, from 760px, the "New Jersey <-> Florida" route label. Both wordmarks (top, footer) link back to the top.

### Hero highway canvas (signature)
A full 2D canvas behind (desktop) or below (phone) the hero copy. Tune it through the `CFG` block at the top of the hero script; don't hand-edit draw code for tuning.
- **Lanes:** 6 on phone, 8 on desktop; upper half warm headlights (`255,236,190`) flowing left, lower half taillight red flowing right. Lane marks: 9% cream dashes, a gold 32% double line at the median.
- **Streaks:** 6 per lane on phone, 11 on desktop; 140-300px/s, 50-150px long, additive blend with a soft 8px glow pass.
- **Road shape:** slow swell (16px phone / 26px desktop) plus 4px ripple; on desktop `TILT .36` sweeps the road up to the right, away from the text. Band `LANE_TOP/LANE_BOT` .10-.62 (phone), .50-.97 (desktop).
- **Car:** cream body, glass-green windows, headlight beams. Autopilot weaves the taillight lanes at 70/95px/s. On touch or hover it follows on a spring (`SPRING 38`, `DAMP 7.5`); lanes part around it (`PUSH 30/40`). After `IDLE_MS 2600` untouched it hands the wheel back. Red trail ribbon behind it.
- **Text clear-zone:** every frame erases a soft-edged (36px blur) rectangle behind the h1, promise and buttons, plus the top bar, and fades the top 16% of the canvas, so no light ever crosses text. Any new hero copy must be added to `measureClear()`.
- **Pre-JS still frame:** two faint CSS gradient trails (gold and red) on the road until the canvas goes live.
- **Hint:** "Drag on the road to drive" (touch) / "Move over the road to drive" (fine pointer), fades out on first interaction.

### Step car on the route rail
In "How it works", the steps hang off a dashed rule-dark rail (58px rail, 72px from 760px) with gold-ringed 14px stops. A top-down car (SVG symbol, pointing south) rides the rail tied to scroll position (60% down the viewport), and the rail fills solid gold behind it via `--done`. Scroll-driven, rAF-throttled, no autonomous loop.

### Motion
- **One loop per element.** The hero canvas runs one rAF loop; all lane seams share one loop. Each pauses via IntersectionObserver when off screen and restarts on re-entry.
- **Reduced motion:** the canvas draws a single still frame (car at 45% across), the hint hides and touch scrolling is restored; seams render their t=0 shape; all CSS transitions collapse to 0.01ms; smooth scroll turns off.
- **Easing:** `--ease-out` `cubic-bezier(.16,1,.3,1)` for lifts, FAQ open, icon turns (0.45-0.5s); color/outline changes 0.2-0.3s linear. Fades are slow (hint 1.2s).

## Do's and Don'ts

### Do:
- **Do** pick color, rule and ring from the ground an element sits on (`on-dark` / `on-light` classes set `--ring`).
- **Do** join every new section to its neighbors with a lane-line divider carrying both grounds' hexes.
- **Do** keep the primary action a `tel:+17323003835` link, gold on green or green on ivory, 60px tall.
- **Do** set facts as ruled lists in serif rows before reaching for cards.
- **Do** keep body copy at 18px+ and measures at 30-40ch.
- **Do** pause any new animation off screen and give it a reduced-motion still frame.
- **Do** put new rates in the stationery card style (paper, double hairline, 6px).

### Don't:
- **Don't** use black or neutral grey anywhere, including shadows.
- **Don't** use taillight red outside moving imagery.
- **Don't** use gold (light) text on ivory or gold-deep on green; it fails contrast on the wrong ground.
- **Don't** wrap sections or list rows in cards; the rates card and the estimate form are the only cards.
- **Don't** add hover fills or color-swap hovers; hover is the outline ring.
- **Don't** let hero copy and light trails overlap; extend the clear-zone instead.
- **Don't** start a second rAF loop for something that can join an existing one.
