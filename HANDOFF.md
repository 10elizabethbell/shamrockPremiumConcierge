# Shamrock Transportation (Vibe 1: premium concierge) — handoff at ~60%

**Live:** https://10elizabethbell.github.io/shamrockPremiumConcierge/ · **Repo:** https://github.com/10elizabethbell/shamrockPremiumConcierge · **Built:** 2026-10-14 from Muse brief of 2026-10-13 (approved by Ellie 2026-10-14)

## What's built
- **World:** a night highway seen from above, like a long-exposure photo. Gold headlight trails flow one way, red taillights the other, on a deep Irish-green ground, with ivory "hotel stationery" sections, muted gold rules and Cormorant Garamond display type (self-hosted in `fonts/`, OFL).
- **Signature element:** in the hero, Ed's car drives itself across the light trails until you touch or hover; then it follows your finger or mouse (every direction, including up and down on phones), and the lanes part around it like traffic making room. It hands the wheel back after 2.6s untouched. On phones the road fills the bottom of the first screen (car visible even at Facebook-browser height, ~390x660); on desktop it sweeps up through the right half and is erased softly behind the headline and buttons so nothing runs through text. Tunable constants sit at the top of the hero script (`CFG`: lanes, streaks, speeds, `LANE_TOP/BOT`, `TILT`, `IDLE_MS`).
- **Carried through the page:** wavy section seams with a gold dashed lane marking painted just inside the lower colour, drifting slowly; in "How it works" a small car rides the dashed route line as you scroll (pointing south) and the line turns solid gold behind it.
- **Sections (brief's order):** hero ("You fly. I'll drive.", from the card's domain youflyilldrive.com) → Pack it full (the #1 differentiator, set as the second-biggest type on the page) → How it works (Call me / Fly / Your car is waiting) → Where I drive + "Very reasonable rates." stationery card (call for your rate, no numbers) → "The man you call is the man who drives" (trust) → FAQ (cost, packing, spring trips, and the honest "when is a trailer carrier better?") → Get your rate (huge tap-to-call number + estimate form) → footer.
- **Contact:** every call link is `tel:+17323003835`. The estimate form validates name/from/to (errors linked to the fields for screen readers) and opens a pre-filled text to the same number (tested: the body decodes correctly). While it opens, the button reads "Opening your messages…", then a line appears with the number in case nothing opened (desktop and some in-app browsers ignore `sms:`). Hero has exactly two buttons: Call Ed (filled gold) and Get your rate (outlined).
- **Reviewed:** Impeccable's detector plus a sweep of every mode except live/onboard, and the finish reviewer (verdict "fix first"); all their material fixes are applied. Detector leftovers are intentional and recorded in `.impeccable/config.json` (tight leading on display headings; green-tinted offset shadow flagged as a glow).
- **Shareables:** `og.png` 1200x630 for the Facebook preview, shamrock favicon (SVG) and `apple-touch-icon.png`.

## Assumptions I made
- **Shamrock mark is drawn by me**, not traced from Ed's card (no card scan was available, and the brief says to ask before using it publicly). It's a simple three-leaf shamrock in a mid green. Swap in the real emblem once Ed or Ellie OKs the card photo.
- **Headline "You fly. I'll drive."** comes from the card's domain (youflyilldrive.com). The promise "so it's waiting when you land" is the brief's concierge line; it implies timing Ed hasn't confirmed.
- **"Every route gets its own flat rate"** follows the brief's "call for your route's flat rate" wording. Ed hasn't said his prices are flat.
- **Pack it full:** "Trailer carriers want the car empty" is a general industry statement (many carriers limit or forbid personal items). The examples (winter clothes, golf clubs, pillows, boxes) are illustrative. I didn't say "free" or give any weight limit.
- **Trust section** ("One driver: me … I'm the one who drives your car", "One car at a time", "The number on this page is my cell") is marked `<!-- CONFIRM WITH ED -->` in the HTML: the brief says Ed is the only *known* driver.
- **"Airport service anywhere in Florida"** is verbatim from the card. I didn't say what it includes (dropping the car at the airport? picking him up?).
- **Footer tagline** "Life is a Highway… Drive it All Night Long" is verbatim from the card. "All night long" might worry a careful 60+ customer, so consider cutting it.
- **Colors:** deep Irish green #11352a and gold #c9a96a, picked from Muse/Ellie's direction rather than sampled from the card.
- **Voice:** first person as Ed ("I").

## Placeholders and gaps
- **Rates (critical):** the rates block is marked with an HTML comment `RATES PLACEHOLDER`. Ed confirms Thursday. Drop the real numbers or the flat-rate table in there.
- No email, Facebook, reviews, photos, hours, insurance or years in business, so those are absent from the page. There's no Facebook link under the work because there are no work photos.
- Texts: "Accepts texts: unknown". The form ("Or text me the details") hands off by SMS, and a call link sits right under it. If Ed doesn't text, change the form button to call, or remove the form.
- No Facebook link under the work or in the footer: there's no Facebook page and no work photos yet (finishing rule waived for lack of a page; add both once he has one).

## Questions for the owner
1. Rates: a flat price per route? Per mile? Seasonal? What's included (gas, tolls, return flight)?
2. Insurance: what covers the car while you drive it? (I left it off the page entirely.)
3. Do you text? (The estimate form opens a text to your cell.)
4. What does "Airport services anywhere in Florida" mean exactly?
5. Is there a limit on what customers can pack (weight, nothing in the driver's view)?
6. Which NJ and FL areas, and how much notice do you need?
7. Can we use your shamrock from the card, and a photo of you (or your car) for the "One driver: me" section?
8. Is youflyilldrive.com yours to register? It's currently unregistered and would make the perfect address for this site.

## Ideas not built (yours to pick)
- **Runner-up world: airport departure board.** A split-flap board flipping "NEWARK → FORT MYERS"-style rows (with real towns once Ed names them), the "airline lounge" polish from the brief. Other worlds considered: an I-95 gold-thread route map, shamrock leaves drifting, hotel valet key tags, rain on a windshield with wipers.
- A season toggle in the hero (South for winter / North for summer) that flips the car's direction and the copy.
- The "Pack it full" list could become a top-down trunk you drag items into.
- A real photo of Ed beside the "One driver: me" line would be the strongest trust signal on the page.
- A rates table once Ed confirms (route → price), styled like the stationery card.
- Overdrive idea from the review: let the hero car's headlight beam brighten the streaks and lane dashes it passes.
- If the hero's `PHONE` layout should switch live when a tablet rotates past 760px, recompute it in `size()` (it's read once at load now).
- Sibling builds `shamrockOwnerTrust` and `shamrockTransparentPricing` were running at the same time. Check that they didn't land on the same highway world.

## Not verified
- Phone screenshots were taken in headless Chrome, which reports a mouse, so they show the desktop hint "Move over the road to drive"; real phones show "Drag on the road to drive".
- Real-device touch in Facebook's in-app browser (iOS and Android). I tested in headless Chrome with simulated touch.
- The SMS handoff on a real iPhone or Android (the `?&body=` form works on both in my experience).
- Frame rate on older phones (the phone draws 6 lanes × 6 streaks).
