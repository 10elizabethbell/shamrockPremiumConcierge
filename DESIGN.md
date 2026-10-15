---
name: Shamrock Transportation
description: One-man NJ <-> Florida driveaway service, premium concierge. Hotel stationery for a night drive, on ivory paper and deep Irish green.
colors:
  ground-deepest: "#0d2b21"
  ground-night: "#11352a"
  ground-journey: "#174233"
  leaf: "#46a96a"
  ivory: "#f5efe2"
  paper: "#fbf8f1"
  ink: "#173a2d"
  ink-soft: "#4a5f55"
  cream: "#efe7d4"
  cream-soft: "#d3dcbd"
  gold: "#c9a96a"
  gold-deep: "#8a6728"
  rule-dark: "rgba(201,169,106,.35)"
  rule-light: "rgba(138,103,40,.32)"
  error: "#a3342a"
typography:
  display:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(50px, 14vw, 84px)"
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: "-0.015em"
  display-wide:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "96px"
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(44px, 12vw, 76px)"
    fontWeight: 600
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(32px, 8.2vw, 42px)"
    fontWeight: 600
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  list-item:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "clamp(28px, 7.4vw, 36px)"
    fontWeight: 500
    lineHeight: 1.2
  route-label:
    fontFamily: "Cormorant, Iowan Old Style, Palatino Linotype, Palatino, Georgia, serif"
    fontSize: "25px"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.01em"
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
  column-gap: "64px"
  wrap: "1160px"
components:
  button-green:
    backgroundColor: "{colors.ground-journey}"
    textColor: "{colors.cream}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "60px"
  text-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.stationery}"
    padding: "0 4px"
    height: "48px"
  route-card:
    backgroundColor: "{colors.ivory}"
    textColor: "{colors.ink}"
    typography: "{typography.route-label}"
    rounded: "{rounded.stationery}"
    padding: "18px 16px 14px"
  honest-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.stationery}"
    padding: "30px 24px 28px"
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

**Creative North Star: "Hotel Stationery for a Night Drive"**

The page is the stationery you'd find in the glovebox of a long night drive: ivory and paper sheets, thin gold rules, a serif that looks engraved, deep Irish green for the night. The first screen is a light paper sheet with a still route card on it, a gold dotted line from New Jersey down to Florida with Ed's car on the line. The night-drive spirit is carried by the green sections, the lane-line seams between them, and the motto from Ed's card in the footer, not by moving imagery.

The page alternates paper and green grounds, joined by wavy lane-line seams: paper hero, ivory "Meet your driver", green rates and text form, deepest-green footer. Structure comes from rules and type, not from boxes: lists are ruled, sections are full-bleed, and only three objects on the page are cards (the route card, the trailer-carrier note, the estimate form). Type is big for a 40-70 reader on a phone: body never under 17px, primary actions 60px tall.

Nothing on the page moves. There is no canvas, no animation loop, no scroll effect; the only transitions are the hover/focus outline ring and a 1px button lift. The audience is 40-70; nothing should need to be learned, dragged or opened to be read.

**Key Characteristics:**
- Light paper hero; deep Irish green sections, never black; ivory and paper for reading sections.
- Cormorant display with one gold italic turn of phrase per heading; system sans for everything read or tapped.
- Thin gold rules, double-hairline stationery cards and still dashed gold lane markings as the only ornament.
- One green pill Call button per block, with an underlined text link as the quieter alternative.
- Completely still: no animation anywhere.

## Colors

A two-ground palette (green night, ivory/paper day) with one metallic accent that shifts tone to stay legible on each ground.

### Primary
- **Muted Lounge Gold** (gold): trim on green. The rates italic and $1, the big phone number, footer motto and wordmark sub-label, lane-line dashes, text selection, the route car's lights.
- **Antique Gold** (gold-deep): the same gold, darkened to read on ivory and paper. Hero italic line, the hero wordmark sub-label, top-bar phone icon, eyebrow text, the route card's dotted line, text-link underline, hover/focus ring on light grounds, input focus border, caret.

### Secondary
- **Shamrock Leaf** (leaf): the shamrock mark only (wordmark and favicon). Not a UI color.

### Neutral
- **Paper** (paper): the hero ground and theme-color; the two cards that sit on ivory or green (trailer-carrier note, estimate form).
- **Ivory** (ivory): paper sections (`on-light`: About) and the route card on the paper hero.
- **Journey Green** (ground-journey): the green button fill; the route card's pins and car body.
- **Night Green** (ground-night): estimate section ground and the page's base background.
- **Deepest Green** (ground-deepest): footer ground.
- **Ink / Ink Soft** (ink, ink-soft): headings, wordmark, phone link and secondary copy on paper/ivory.
- **Cream / Cream Soft** (cream, cream-soft): headings and secondary copy on green; cream-soft also paints the route car's windows.
- **Rule Dark / Rule Light** (rule-dark, rule-light): 1px gold hairlines; dark on green, light on ivory/paper.
- **Error Brick** (error): field error border and message. Hardcoded in CSS, not yet on `:root`; promote it if more states appear.

The old night-highway colors are retired: taillight red is gone with the canvas, and the glass-green car-window tone (`--g-700`) has been removed from `:root`.

### Named Rules
**The Never-Black Rule.** The darkest value on the page is ground-deepest. No `#000`, no neutral greys; shadows are tinted from the ground green.

**The Ground-Matched Gold Rule.** On green, use gold; on ivory or paper, use gold-deep. Same for rules (rule-dark vs rule-light) and text (cream vs ink). Every element picks its pair from the ground it sits on, never across. The lane-line dashes are the one exception: they are road paint, always gold, never text.

## Typography

**Display Font:** Cormorant (Cormorant Garamond, self-hosted latin subset in `fonts/`, weights 500-700 roman and italic) with Iowan Old Style / Palatino / Georgia fallback.
**Body Font:** system sans stack (-apple-system, Segoe UI, system-ui).

**Character:** an engraved, high-contrast serif for everything said, a plain native sans for everything read at length or tapped. The serif is big and tight; the sans is big and loose.

### Hierarchy
- **Display**: hero h1 only, ink. Second line italic 500 in gold-deep, on its own line. Steps to Display Wide (fixed 96px) from 1100px.
- **Headline**: section h2, below the hero h1; the about h2 drops to `clamp(40px, 10.5vw, 64px)`.
- **Title**: h3 for the trailer-carrier note and form titles (28-38px by context).
- **List item**: ruled serif rows (about facts 600 at `clamp(24px, 6.4vw, 30px)` / 1.25).
- **Route label**: serif 600 at 25px inside the route card ("New Jersey", "Florida"); the wordmark "Shamrock" is set at the same size (28px in the footer, 22px under 370px).
- **Phone number**: serif 600 `clamp(42px, 12vw, 72px)`, lining tabular figures, gold. The number is set as type, not as a button.
- **Lede**: one sentence under an h2, max 34ch, soft color. The hero promise is a lede at 18-21px, max 32ch.
- **Body**: 18px / 1.6 (19px from 760px). Measure 30-40ch.
- **Label**: uppercase tracked sans, 12.5-15px, 0.12-0.2em. Only for the wordmark's "Transportation".

### Named Rules
**The One Italic Rule.** Each heading may turn one phrase italic 500, colored gold (green ground) or gold-deep (paper/ivory). That phrase carries the meaning ("I'll drive.", "full.", "rates."). Never italicize a whole paragraph.

**The 17px Floor.** Nothing the customer reads drops below 17px (16px only for the copyright line). Labels are the one smaller register, and they are never sentences.

**Tight Serif, Loose Sans.** Serif headings sit at 0.95-1.25 line height; sans copy at 1.5-1.6. The tight leading on display is intentional.

## Layout

Single-scroll, phone-first one-pager. Content sits in a centered wrap (max 1160px) with a side gutter of 20px (16px under 370px, 40px from 760px). Sections are full-bleed grounds with vertical padding of 64/72px on phones and 104/112px from 760px.

**Breakpoints** (min-width unless noted):
- **base (phone)**: everything stacks; the hero Call button is full-width (max 420px) with the text link beside or under it; the route card sits below the hero copy.
- **max 370px**: narrower gutter, smaller button text and padding, smaller wordmark and phone link.
- **760px**: gutter 40px, body 19px, top-bar nav links appear the hero goes two-column (copy left, route card right, 64px gap), the Call button sizes to content, footer 3 columns. Lane seams 44 to 60px tall.
- **960px**: about and estimate go two-column (64px gap).
- **1100px**: hero h1 fixed at 96px.

**The Ruled List Rule.** Lists of facts (about facts) are rows separated by 1px rules, top rule on the first item, no bullets, no boxes. Row padding 14-16px vertical.

**No Hidden Content Rule.** Nothing is tucked behind an accordion, tab or tap. Every answer is visible as you scroll.

## Elevation & Depth

Mostly flat: depth comes from the ground alternation and from the stationery cards sitting one step off their ground. Shadows are soft, long and negatively spread.

### Shadow Vocabulary
- **Soft** (`--shadow-soft`): green button. Its alpha is currently mixed from black, which breaks the Never-Black Rule; retint it from ground-deepest (`rgba(6,26,19,…)`) like the form float. Do not copy the black value.
- **Form float** (`0 30px 60px -30px rgba(6,26,19,.6)`): estimate form on green.

The route card and trailer-carrier note carry no shadow; they are flat stationery defined by their double hairline.

**The Lit-From-Above Rule.** Every shadow falls straight down with a negative spread, so it reads as ambient light under an object, never a hard offset or a glow halo.

## Shapes

Round where you touch, square-ish where you read. Buttons are full pills (999px); the direction contract said "no pills", but the build ships pill buttons and they are recorded here as the system (no pill-shaped chips or tags exist). Inputs are gently rounded (12px), the estimate form generously (22px). The route card and trailer-carrier note are near-square (6px), drawn as stationery: a 1px rule-light border plus a second 1px rule inset 9px (outline with negative offset), the double-ruled border of a hotel card. Focus rings round to 4px. Dividers are never straight lines between grounds: see Lane-line dividers.

## Components

### Buttons
- **Shape:** full pill (999px), 60px min height, 26px side padding, 21px leading SVG phone icon, 1.5px border.
- **Green:** journey-green fill, cream text, soft shadow. The only button variant: the hero Call Ed button (number inside in tabular figures at 85% opacity) and the form submit.
- **Hover / Focus:** a 2px outline ring at 3px offset in the ground's ring color, plus a 1px lift; press drops 1px. Transform and shadow ease over 0.5s on `cubic-bezier(.16,1,.3,1)`.
- One button per block. The hero has exactly one (Call), with the text link as the alternative.

### Text link
The quieter alternative to a button ("or text me instead"): 18px 600 sans in ink, underlined in gold-deep at a 4px offset, 48px tall tap target. Hover and focus take the outline ring.

**The One Ring Rule.** Hover and keyboard focus look the same: a 2px outline at a small offset. Sections set `--ring` (`on-dark`: cream; `on-light` and the form: gold-deep) and every interactive thing (buttons, text link, top-bar links, big number, footer and form links, inputs) uses it. Don't introduce color-fill hovers.

### Route card (hero)
Ivory stationery card on the paper hero: double gold hairline, 6px radius, padding 18/16/14 (28/26/22 from 760px), no shadow. Holds an inline SVG (max 440px wide): a gold-deep dotted route (2.5px, dash 2/9, round caps) curving from a New Jersey pin down to a Florida pin, journey-green pins with paper centers, Ed's car (journey-green body, cream-soft windows, gold lights) sitting still on the line, labels in the route-label serif. It has `role="img"` and an aria-label. It is a placeholder slot: when Ed supplies a photo, the photo replaces the SVG inside the same card.

### Lane-line dividers (signature)
A 44px (60px from 760px) SVG seam between every pair of grounds, including hero (paper) to Meet your driver (ivory). The upper ground fills the background, the lower ground fills a gently waving path, and a gold dashed line (3px, dash 26/18, round caps) runs 11px inside the lower color like a road marking. The wave (amplitude 7px) and dashes are still; they are drawn once and redrawn only on resize. Set `data-from` / `data-to` to the two grounds' hexes. Every section boundary uses one; never a straight edge or an `<hr>`.

### Ruled lists
About facts (serif rows: routes and services from the card).

### Trailer-carrier note (stationery)
Paper on ivory, double gold hairline border, 6px radius, padding 30/24/28 (40/38/36 from 760px). Ink h3, a short bulleted list, one closing line. The real rates table, once Ed confirms, should use this same card style inside the rates section.

### Price line
In the rates section, under the h2: one row between two 1px rule-dark rules. "$1" in the serif at `clamp(64px, 17vw, 96px)` 600, gold, lining figures, followed by "per mile" in the serif at `clamp(28px, 7.4vw, 36px)` 500, cream, sharing a baseline. A plain sans sentence under it asks the reader to call for the exact price. Keep price changes in this row; don't add a pricing table or calculator without real route mileages from Ed.

### Estimate form
Paper card on green, 22px radius, form-float shadow, sets `--ring: gold-deep`. Labels 18px 600 ink above fields; "(optional)" set in normal-weight ink-soft. Inputs white, 1.5px ink-at-28% border, 12px radius, 56px min height; hover and focus switch border and outline to gold-deep. Errors: brick border plus a 17px brick message under the field, linked with `aria-describedby`. Submit is a full-width green button. It composes an SMS, not a server post.

### Navigation
The top bar is the shamrock wordmark (leaf-green mark, serif "Shamrock", tracked "Transportation") on the left. No phone number in the top bar (Ellie, 2026-10-15): the hero's Call Ed button carries it, so it isn't repeated. On the paper hero the wordmark is ink with a gold-deep sub-label; in the footer it is cream with a gold sub-label. From 760px two plain text links (17px 500, ink-soft) sit on the right: Meet Ed, Rates. No menu button, no dropdown. Both wordmarks link back to the top.

### Eyebrow
The build carries two sentence-case lines in 17px 600 sans gold-deep above a heading: the hero ("Personal car delivery · New Jersey & Florida" at every width, the place name kept on one line) and "Meet your driver" above the about h2. **The Eyebrow Rule.** These two are the limit: add no new eyebrows, and never set one in caps or tracking. A new section introduces itself with its heading.

### Motion
**The Still Page Rule.** Add no animation. No canvas, no rAF loop, no scroll-triggered effects, no autoplay, no moving imagery. The only transitions allowed are the hover/focus outline ring (0.2s), color and border changes (0.2-0.3s), and the 1px button lift (0.5s on `--ease-out`). Under reduced motion, transitions collapse to 0.01ms and smooth scroll turns off.

## Do's and Don'ts

### Do:
- **Do** pick color, rule and ring from the ground an element sits on (`on-dark` / `on-light` classes set `--ring`).
- **Do** join every new section to its neighbors with a lane-line divider carrying both grounds' hexes.
- **Do** keep the primary action a `tel:+17323003835` link in the green pill button, 60px tall, one per block.
- **Do** set facts as ruled lists in serif rows before reaching for cards.
- **Do** keep body copy at 18px+ and measures at 30-40ch.
- **Do** swap Ed's photo into the route card when supplied, keeping the ivory double-hairline frame.
- **Do** keep the price in the rates section's price line; if Ed adds inclusions (gas, tolls, flight), list them as one plain sentence under the price line.

### Don't:
- **Don't** add animation of any kind; the page is still.
- **Don't** use black or neutral grey anywhere, including shadows.
- **Don't** use gold (light) text on ivory or paper, or gold-deep on green; it fails contrast on the wrong ground.
- **Don't** wrap sections or list rows in cards; the route card, the trailer-carrier note and the estimate form are the only cards.
- **Don't** add hover fills or color-swap hovers; hover is the outline ring.
- **Don't** add more eyebrows above headings.
- **Don't** make anything draggable, hover-driven or hidden behind a tap; this audience shouldn't have to discover how the page works.
