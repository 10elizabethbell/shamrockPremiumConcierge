# Shamrock Transportation (Vibe 1: premium concierge) — handoff at ~60%

**Live:** https://10elizabethbell.github.io/shamrockPremiumConcierge/ · **Repo:** https://github.com/10elizabethbell/shamrockPremiumConcierge · **Built:** 2026-10-14 from Muse brief of 2026-10-13 (approved by Ellie 2026-10-14)

## What's built
- **World:** hotel stationery for a night drive: ivory paper and deep Irish green, muted gold rules, still dashed road-marking seams between sections, Cormorant Garamond display type (self-hosted in `fonts/`, OFL).
- **Hero (replaced 2026-10-14, Ellie: the night-highway hero was too much for this audience):** light paper first screen with the headline, one sentence naming Ed, ONE green Call button, an "or text me instead" link, and a still route card (gold dotted line from a New Jersey pin to a Florida pin with Ed's car on it). It's built to swap for a photo of Ed beside a car once he supplies one. **Nothing on the page animates now:** the hero canvas and its script are deleted.
- **Carried through the page:** still, wavy section seams with a gold dashed lane marking painted just inside the lower colour. Nothing below the hero moves.
- **Simplified 2026-10-14 (Ellie: audience is 40-70, first version was too much):** removed the drivable car, the drag hint, the moving seams and the scroll-driven step car; cut "Where I drive", the separate rates card, the 3-part trust list and the FAQ accordion (no hidden content now); form cut from 6 fields to 4 with plain-question labels.
- **Sections (3 + footer):** hero ("You fly. I'll drive.", from the card's domain youflyilldrive.com; eyebrow says the service, promise names Ed) → "The man you call is the man who drives" (Ed, one car at a time, the card's services as a short list, plus a visible note on when a trailer carrier is the better choice) → "Very reasonable rates." ($1 per mile, huge tap-to-call number, text form) → footer.
- **Contact:** every call link is `tel:+17323003835`. The estimate form (name, where the car is, where it's going, optional when) validates the three required fields (errors linked to the fields for screen readers) and opens a pre-filled text to the same number (tested: the body decodes correctly). While it opens, the button reads "Opening your messages…", then a line appears with the number in case nothing opened (desktop and some in-app browsers ignore `sms:`). Hero has exactly two buttons: Call Ed (filled gold) and Get your rate (outlined).
- **Reviewed:** Impeccable's detector plus a sweep of every mode except live/onboard, and the finish reviewer (verdict "fix first"); all their material fixes are applied. Detector leftovers are intentional and recorded in `.impeccable/config.json` (tight leading on display headings; green-tinted offset shadow flagged as a glow).
- **Shareables:** `og.png` 1200x630 for the Facebook preview (currently the light hero with the route card), shamrock favicon (SVG) and `apple-touch-icon.png`.

## Research brief applied (2026-10-14)
Ellie's "Designing for trust, clarity, and effortless contact" brief (ages 40-70) was applied where it fits the vibe and the facts we have:
- Header: Ed's number as a tap-to-call link on every screen size; desktop adds 2 plain links (Meet Ed, Rates).
- Hero answers what / who / where / contact in one screen: eyebrow "Personal car delivery · New Jersey & Florida", promise now opens "I'm Ed Brannagan" and says you talk to him directly. Second action is now an "or text me instead" link (jumps to the text form).
- "Meet your driver" label over the about section; form now says what happens next ("I'll get back to you with your rate").
- Not applied, on purpose:
  - **Sticky mobile Call button:** conflicts with your no-sticky-bar rule. The number is in the header and the first button instead. Your call.
  - **Portrait / Meet Your Driver photo, reviews, insurance, credentials, pricing inclusions, insurance/timing/mileage FAQ:** need real facts from Ed. Not invented; listed in the questions below.
  - **Inter / Atkinson body font, warm-white page, 32-48px headings:** would replace the premium vibe you asked to keep. Body is already system sans at 18-19px; the big serif headings stay.
  - **"Free quote" wording:** Ed hasn't said quotes are free; buttons say "Call Ed" and "rate".

## Assumptions I made
- **Shamrock mark is drawn by me**, not traced from Ed's card (no card scan was available, and the brief says to ask before using it publicly). It's a simple three-leaf shamrock in a mid green. Swap in the real emblem once Ed or Ellie OKs the card photo.
- **Headline "You fly. I'll drive."** comes from the card's domain (youflyilldrive.com). The promise "so it's waiting when you land" is the brief's concierge line; it implies timing Ed hasn't confirmed.
- **About section** ("I drive one car at a time, and the number on this page is my cell") is marked `<!-- CONFIRM WITH ED -->` in the HTML: the brief says Ed is the only *known* driver.
- **"Airport service anywhere in Florida"** is verbatim from the card. I didn't say what it includes (dropping the car at the airport? picking him up?).
- **Footer tagline** "Life is a Highway… Drive it All Night Long" is verbatim from the card. "All night long" might worry a careful 60+ customer, so consider cutting it.
- **Colors:** deep Irish green #11352a and gold #c9a96a, picked from Muse/Ellie's direction rather than sampled from the card.
- **Voice:** first person as Ed ("I").

## Placeholders and gaps
- **Ed's photo (placeholder, Ellie 2026-10-14):** the hero's route card and the Facebook preview `og.png` both stand in for a photo of Ed. When it arrives: put it in the hero in place of `.route-card` (same right-hand column on desktop, below the Call button on phones), and re-render `og.png` with Ed's photo on the right in place of the route card. Then run the link through Facebook's Sharing Debugger ("Scrape again"), because Facebook caches the old preview.
- **Price is $1 per mile** (Ed via Ellie, 2026-10-15), marked with a `RATES` HTML comment. What it includes is still unknown and not on the page.
- No email, Facebook, reviews, photos, hours, insurance or years in business, so those are absent from the page. There's no Facebook link under the work because there are no work photos.
- Texts: "Accepts texts: unknown". The form ("Or text me the details") hands off by SMS, and a call link sits right under it. If Ed doesn't text, change the form button to call, or remove the form.
- No Facebook link under the work or in the footer: there's no Facebook page and no work photos yet (finishing rule waived for lack of a page; add both once he has one).

## Questions for the owner
1. Rates: $1 per mile confirmed. Is there a minimum, or a different spring/fall price? What's included (gas, tolls, your flight back)?
2. Insurance: what covers the car while you drive it? (I left it off the page entirely.)
3. Do you text? (The estimate form opens a text to your cell.)
4. What does "Airport services anywhere in Florida" mean exactly?
5. Is there a limit on what customers can pack (weight, nothing in the driver's view)?
6. Which NJ and FL areas, and how much notice do you need?
7. Can we use your shamrock from the card, and a photo of you (or your car) for the "One driver: me" section?
8. Is youflyilldrive.com yours to register? It's currently unregistered and would make the perfect address for this site.
9. A portrait of you (and one beside a car) for the hero and "Meet your driver"; years driving; why you do this work, in your words.
10. Two or three customers who'd let us quote them by name.
11. What's in the price: gas, tolls, lodging, your flight back? And what happens if something goes wrong on the road?

## Ideas not built (yours to pick)
- **The old night-highway hero** (animated light trails with Ed's car) is in git history (commit c796a10) if you ever want it for a different, younger-skewing pitch.
- **Runner-up world: airport departure board.** A split-flap board flipping "NEWARK → FORT MYERS"-style rows (with real towns once Ed names them), the "airline lounge" polish from the brief. Other worlds considered: an I-95 gold-thread route map, shamrock leaves drifting, hotel valet key tags, rain on a windshield with wipers.
- A season toggle in the hero (South for winter / North for summer) that flips the car's direction and the copy.
- A real photo of Ed beside the "One driver: me" line would be the strongest trust signal on the page.
- A few sample routes with mileage and price (e.g. "Toms River → Naples") once Ed names his usual towns, so readers see real numbers without calling.
- If the hero's `PHONE` layout should switch live when a tablet rotates past 760px, recompute it in `size()` (it's read once at load now).
- Cut in the simplification, easy to restore from git history if wanted: the "Pack it full" section (cut 2026-10-14; commit e76e727 has it), the "How it works" steps (cut 2026-10-15; commit 48416c8 has them), the drivable hero car, the FAQ accordion, the trust three-up, the scroll car in "How it works", the optional Car and Notes form fields.
- Sibling builds `shamrockOwnerTrust` and `shamrockTransparentPricing` were running at the same time. Check that they didn't land on the same highway world.

## Not verified
- The SMS handoff on a real iPhone or Android (the `?&body=` form works on both in my experience).
