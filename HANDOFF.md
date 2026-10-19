# Gutter Guys — handoff at ~60%

**Live:** https://10elizabethbell.github.io/gutterGuys/ · **Repo:** https://github.com/10elizabethbell/gutterGuys · **Built:** 2026-10-18 from Muse brief (run 2026-10-18, Facebook group "Essex County Contractor Referrals")

## What's built
- One page, `index.html` (inline CSS/JS, system fonts, no tracking). Assets in `assets/` (logo, favicon, touch icon, og image), ~100KB plus the 133KB og image.
- **World:** the page is a house's drainage system on a rainy fall evening. Deep navy, Gutter Guys royal blue, aluminium-white trough and downspout, slate shingles, wet amber/rust leaves.
- **Signature (hero canvas):** an eavestrough packed with leaves under a shingled roof, with rain falling. Wherever leaves block the trough, water spills over the front lip. Where it's clear, water runs to the downspout and pours out the elbow, and the stream grows as the gutter clears. Drag a finger (any direction; the canvas owns its touches) or move the mouse to scoop the leaves out. They tumble down, and new leaves drift back in slowly (`REGROW`). Until someone touches it, it clears a third of the gutter on its own every ~5.5s. Tunables are at the top of the hero IIFE (`CFG`).
- **Water seams:** animated three-line water waves between every section, with the fill following the middle line.
- **Sections:** header (logo + name, 519-991-2813 top-right) → hero (headline, promise, "Get a free quote" + "Text us a photo") → What we clean (8 rows; each jumps to the form with that service ticked) → Don't wait for the damage (their 4 flyer claims) + How it works (3 steps) + "See our latest jobs" Facebook button → Get your free quote form → footer (both numbers, Facebook, "Residential · Commercial · Fully insured").
- **Contact wiring:** the form composes a text to +1 519-991-2813 (`sms:...?&body=`), with inline errors and both numbers to call underneath. "Text us a photo" opens a text with a starter message. Tested: SMS bodies encode and decode correctly (apostrophes, &, #, %, ?).

## Assumptions I made
- **Voice "we":** the brief says business page, no owner name, and "Guys" is plural.
- **Primary number 519-991-2813:** listed first on both the flyer and the caption. 519-778-1752 appears only in the form note and the footer.
- **Texting:** accepts-texts is *unknown*. Texting is a primary path, but calling is always one tap away (header, form note, footer).
- **Colors** were sampled by eye from the logo and flyer (royal blue `#2563d9`, navy ground instead of the logo's black).
- **"Fully insured", "Residential · Commercial":** printed on their flyer's bottom strip but missing from the brief's OCR. Confirm both.
- **Service names** are shortened from the caption and flyer (e.g. "Soffit & fascia", "Minor gutter repairs" from "GUTTER REPAIRS (minor)").
- **Promise line** ("We work on your roof like it's our own, and we don't pack up until the last leaf is off your lawn.") and the How it works copy are mine, grounded in their "Complete ground cleanup" service. Rewrite them in the owner's words.
- **Favicon** is the three water drops from the logo, and the touch icon is the full badge.

## Placeholders and gaps
- **No work photos.** The flyer's six before/after tiles look AI-generated (same composition style, different houses in some pairs) and are ~90px each, so they're not used as proof. The Facebook button stands in for proof.
- **No service area on the page.** The 519 area code is SW Ontario, but the ad ran in a New Jersey group. The brief says don't publish one.
- No hours, owner name, email, reviews or prices, so the page says nothing about them (and has no footer email).
- No higher-resolution logo than the 720px Facebook profile image.

## Questions for the owner
1. Which towns do you serve? (Then add a plain-text service-area line.)
2. Do both numbers take texts? Which one should quotes go to?
3. Can you send real before/after photos? Same spot, before and after.
4. Are you insured? Do you do commercial jobs?
5. Your first name(s), so the page can say who shows up?
6. Hours and an email, if you want them listed?
7. Which services matter most this season, so they go first?

## Ideas not built (yours to pick)
- **Runner-up world:** moss and black streaks on a shingle roof that you scrub clean, with grime regrowing (the Above All recipe). Good for leading with roof cleaning in spring.
- Before/after sliders under the services once real photos exist.
- A first-touch hint ("Drag along the gutter") if people don't realise it's touchable. The self-play reads a bit like wind.
- A visible scoop or gloved hand for the self-play sweep.
- A small splash when a service chip is ticked (Sunny Side liked it).
- Overflow drips could get round heads so they read less like rain.
- A desktop-only "or text 519-991-2813" under the photo button (it does nothing without a phone), but that would show the number twice on screen.
- Seasonal headline swap (fall: "Leaves in the gutter?").
- Audience age isn't in the brief. If the owner says most customers are 50+, switch to `older-audience.md` (still scene, no self-play).

## Review status
- Impeccable: detector run (two findings left on purpose, with ignores recorded in `.impeccable/config.json`: the hairline row divider and body-tier type sizes). An all-modes sweep (critique, audit, polish, distill, harden, clarify, adapt, optimize, typeset, layout, colorize, animate, delight, bolder, quieter, overdrive) with its fixes applied. Finish reviewer: two rounds. Round 1 fixes were scored 6 resolved, 1 partial. Round 2 fixes (overflow as translucent sheets that break into drops, the desktop downspout outlet above the fold, the repeated "our own" line removed) were applied but **not re-scored** (the unattended budget is two rounds).
- The finishing-rules checklist was re-checked after the sweep.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser). A Chromium CDP touch drag cleared 127→0 leaves without scrolling the page, and the mouse sweep worked. WebKit renders correctly, but its synthetic touch couldn't be driven.
- The real SMS handoff opening Messages with the body on iOS and Android.
- Frame rate on older phones (phone draws ~125 leaves + ~60 rain streaks; one shared loop that pauses off screen).
- The Facebook og preview on a real post (og image is set, but FB's scraper cache wasn't checked).
