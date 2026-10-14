# Shamrock Transportation (Vibe 1: premium concierge) — handoff at ~60%

**Live:** https://10elizabethbell.github.io/shamrockPremiumConcierge/ · **Repo:** https://github.com/10elizabethbell/shamrockPremiumConcierge · **Built:** 2026-10-14 from Muse brief of 2026-10-13 (approved by Ellie 2026-10-14)

## What's built
- **World:** a night highway seen from above, like a long-exposure photo. Gold headlight trails flow one way, red taillights the other, on a deep Irish-green ground, with ivory "hotel stationery" sections, muted gold rules and Cormorant Garamond display type (self-hosted in `fonts/`, OFL).
- **Signature element:** in the hero, Ed's car drives itself across the light trails until you touch or hover; then it follows your finger or mouse (every direction, including up and down on phones), and the lanes part around it like traffic making room. It hands the wheel back after 2.6s untouched. Tunable constants sit at the top of the hero script (`CFG`).
- **Carried through the page:** wavy gold dashed lane-line dividers between sections that flow like road markings; a small car rides the dashed route line in "How it works" as you scroll (pointing south).
- **Sections (brief's order):** hero ("You fly. I'll drive.", from the card's domain youflyilldrive.com) → Pack it full (the #1 differentiator) → How it works (Call me / Fly / Your car is waiting) → Where I drive + Rates (call-for-your-rate block, no numbers) → "The man you call is the man who drives" (trust) → FAQ (including the honest "when is a trailer carrier better?") → Get your rate (huge tap-to-call number + estimate form) → footer.
- **Contact:** every call link is `tel:+17323003835`. The estimate form validates name/from/to and opens a pre-filled text to the same number (tested: the body decodes correctly). Hero has exactly two buttons: Call Ed (filled gold) and Get a rate estimate (outlined).
- **Shareables:** `og.png` 1200x630 for the Facebook preview, shamrock favicon (SVG) and `apple-touch-icon.png`.

## Assumptions I made
- **Shamrock mark is drawn by me**, not traced from Ed's card (no card scan was available, and the brief says to ask before using it publicly). It's a simple three-leaf shamrock in a mid green. Swap in the real emblem once Ed or Ellie OKs the card photo.
- **Headline "You fly. I'll drive."** comes from the card's domain (youflyilldrive.com). The promise "so it's waiting when you land" is the brief's concierge line; it implies timing Ed hasn't confirmed.
- **"Every route gets its own flat rate"** follows the brief's "call for your route's flat rate" wording. Ed hasn't said his prices are flat.
- **Pack it full:** "Trailer carriers want the car empty" is a general industry statement (many carriers limit or forbid personal items). The examples (winter clothes, golf clubs, pillows, boxes) are illustrative. I didn't say "free" or give any weight limit.
- **"One car at a time"** is true for any one-person driveaway trip, but it's still worth confirming with Ed.
- **"Airport service anywhere in Florida"** is verbatim from the card. I didn't say what it includes (dropping the car at the airport? picking him up?).
- **Footer tagline** "Life is a Highway… Drive it All Night Long" is verbatim from the card. "All night long" might worry a careful 60+ customer, so consider cutting it.
- **Colors:** deep Irish green #11352a and gold #c9a96a, picked from Muse/Ellie's direction rather than sampled from the card.
- **Voice:** first person as Ed ("I").

## Placeholders and gaps
- **Rates (critical):** the rates block is marked with an HTML comment `RATES PLACEHOLDER`. Ed confirms Thursday. Drop the real numbers or the flat-rate table in there.
- No email, Facebook, reviews, photos, hours, insurance or years in business, so those are absent from the page. There's no Facebook link under the work because there are no work photos.
- Texts: "Accepts texts: unknown". The form hands off by SMS, and a call link sits right under it. If Ed doesn't text, change the form button to call, or remove the form.

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
- A rates table once Ed confirms (route → price), styled like a hotel rate card.
- Sibling builds `shamrockOwnerTrust` and `shamrockTransparentPricing` were running at the same time. Check that they didn't land on the same highway world.

## Not verified
- Real-device touch in Facebook's in-app browser (iOS and Android). I tested in headless Chrome with simulated touch.
- The SMS handoff on a real iPhone or Android (the `?&body=` form works on both in my experience).
- Frame rate on older phones (the phone draws 6 lanes × 6 streaks).
