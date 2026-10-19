---
name: Gutter Guys
description: A house's drainage path on a rainy fall evening, cleared by the visitor's own finger.
colors:
  navy: "#0c1a33"
  navy-2: "#10244a"
  navy-3: "#163063"
  blue: "#2563d9"
  blue-press: "#1c4fb5"
  blue-hi: "#7fb0ff"
  leaf: "#e7a23b"
  focus: "#b96f14"
  mist: "#e8eff8"
  white: "#ffffff"
  ink: "#eef3fb"
  ink-dim: "#b4c4de"
  ink-dark: "#0f2140"
  ink-dark-dim: "#3b5378"
  rule: "#c3d1e4"
  rule-on-navy: "rgba(127,176,255,.22)"
  field-steel: "#8597b4"
  error-brick: "#a3261b"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2.15rem, 9.4vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2rem, 8.6vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  subhead:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1.6rem, 6.4vw, 2.4rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "20px"
    fontWeight: 800
    lineHeight: 1.35
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(18px, 4.8vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"SF Pro Display\", \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1.4
rounded:
  field: "12px"
  button: "14px"
  full: "50%"
spacing:
  gutter: "16px"
  max: "1180px"
  stack-sm: "12px"
  stack-md: "22px"
  section-y-phone: "44px 0 56px"
  section-y-desktop: "72px 0 88px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.white}"
    rounded: "{rounded.button}"
    padding: "0 26px"
    height: "58px"
  button-primary-hover:
    backgroundColor: "{colors.blue-press}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.button}"
    padding: "0 26px"
    height: "58px"
  input-text:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink-dark}"
    rounded: "{rounded.field}"
    padding: "14px"
    height: "54px"
  chip:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink-dark}"
    rounded: "{rounded.field}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.navy-2}"
    textColor: "{colors.white}"
  service-row:
    textColor: "{colors.ink-dark}"
    typography: "{typography.title}"
    padding: "8px 2px"
    height: "64px"
  service-row-arrow:
    rounded: "{rounded.full}"
    textColor: "{colors.ink-dark}"
    size: "42px"
  service-row-arrow-hover:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.white}"
  tel-link:
    textColor: "{colors.ink}"
    height: "44px"
    padding: "0 4px"
---

# Design System: Gutter Guys

## Overview

**Creative North Star: "The Drainage Path"**

The page is a house's drainage system on a rainy autumn evening. Water enters at the roofline in the hero, where a leaf-packed aluminium eavestrough overflows until the visitor clears it with a finger or mouse; it then runs down the page through animated water seams between sections and ends at the quote form. Every section is a stretch of that path, alternating between rainy-evening navy and a pale washed-mist ground.

The system is plain and loud the way a crew's truck lettering is plain and loud: heavy italic uppercase headings echoing the logo badge, one royal blue for action, and wet autumn leaves (amber, rust, brown) as the only warm color. Density is phone-first and one-handed: big tap targets (44px floor, 58px buttons), full-width actions on phone, single column until 1024px.

It rejects the category default: no stock-photo hero, no blue checkmark list, no "Call Now" banner or sticky call bar. Proof is the visitor doing the job, not a claimed photo.

**Key Characteristics:**
- Navy ground that is never black; light sections are mist, never pure white.
- Heavy (900) italic uppercase display lettering with tight tracking.
- One action blue; amber leaf is the only warm hue and doubles as the focus and selection color.
- Animated water seams join every section change.
- Lists are hairline-divided rows, never boxed cards.
- The hero is an interactive canvas scene, not an image.

## Colors

A cool two-ground palette (deep navy and pale mist) with one saturated royal blue for action and a single warm leaf amber held back for focus, selection and the scene's leaves.

### Primary
- **Gutter Guys Royal** (blue): the logo's royal blue. Filled buttons, the service-row arrow on hover, the brightest stroke in the water seams.
- **Pressed Royal** (blue-press): hover and press state of filled buttons only.
- **Rain-Light Blue** (blue-hi): the second line of the hero headline, step numerals, the header phone icon, footer link hover, and the mid seam stroke. The blue that reads on navy.

### Secondary
- **Wet Leaf Amber** (leaf): the only warm color. Focus ring on navy grounds, text selection, caret, the check glyph in selected chips, header phone icon on hover. Never a fill for large areas.
- **Burnt Leaf** (focus): the darker amber used for focus and hover outlines on mist grounds (inputs, chips, submit), where the lighter leaf would not hold contrast.

### Neutral
- **Rainy-Evening Navy** (navy): page and footer ground, theme color, the hero's bottom stop.
- **Deep Gutter Navy** (navy-2): dark mid-page sections and the selected-chip fill.
- **Downspout Navy** (navy-3): scrollbar thumb.
- **Washed Mist** (mist): light section ground.
- **Trough White** (white): field and chip fills, logo disc.
- **Rain Ink** (ink) and **Dim Rain Ink** (ink-dim): primary and secondary text on navy.
- **Slate Ink** (ink-dark) and **Dim Slate Ink** (ink-dark-dim): primary and secondary text on mist.
- **Mist Rule** (rule): 1px dividers and arrow-circle strokes on mist.
- **Navy Rule** (rule-on-navy): 1px dividers on navy.
- **Field Steel** (field-steel): 2px resting stroke on inputs and chips.
- **Brick** (error-brick): validation message text and invalid field stroke.

### Named Rules
**The Never-Black Rule.** The darkest ground is Rainy-Evening Navy. No #000 surfaces or text anywhere, including the scene.

**The One Warm Color Rule.** Amber belongs to the leaves. It appears in the UI only as focus, selection, caret and the selected-chip check; it is never a button, banner or section fill.

**The Two Grounds Rule.** Sections alternate navy / mist, and every change between them is a water seam, never a hard edge.

## Typography

**Display Font:** system stack (-apple-system, SF Pro Display, Segoe UI, Roboto, Helvetica Neue, Arial)
**Body Font:** the same system stack

**Character:** One family carried at two extremes: 900-weight italic uppercase for anything that names a thing, plain 400 sentence case for anything that explains. The italic slant and tight tracking echo the logo badge's lettering. The build ships the system stack to stay a single request-free file; the treatment (900, italic, uppercase, -0.02em, 0.95 line height) is the system, the face is replaceable by a heavy italic display face if one is licensed.

### Hierarchy
- **Display** (900 italic uppercase, clamp(2.15rem, 9.4vw, 5.6rem); clamp to 6.6vw / 6rem at 1024px+; 0.95): hero headline only, two lines, the second in Rain-Light Blue.
- **Headline** (900 italic uppercase, clamp(2rem, 8.6vw, 3.6rem), 0.95): section h2s.
- **Subhead** (900 italic uppercase, clamp(1.6rem, 6.4vw, 2.4rem), 0.95): h3s inside a section ("How it works", "See our latest jobs").
- **Title** (800, 20px, 1.35): service rows, benefit items, step leads.
- **Lede** (400, clamp(18px, 4.8vw, 20px), 1.5, 34-40ch): the line under a headline, in the dim ink of its ground.
- **Body** (400, 18px, 1.55): base text; form labels and legends at 800/18px.
- **Label** (700, 16px): trust line, footer, chips, validation messages, the form's after-note. 16px is the floor; nothing smaller.

### Named Rules
**The Shout-Then-Speak Rule.** Headings are always 900 italic uppercase; nothing below a heading is uppercase or italic. There are no small-caps labels, eyebrows or tracked-out kickers.

**The Numeral Rule.** Step numbers are 40px 900 italic numerals in Rain-Light Blue, set in a 44px gutter column; never circles or badges.

## Layout

Single column at phone widths inside a 16px gutter, max container 1180px. Sections pad 44px top / 56px bottom on phone, 72 / 88 at 1024px+. Vertical rhythm inside sections steps 12 / 22 / 52-56px.

- **Hero:** fills min(100svh, 920px) as a flex column: header, copy, then the gutter scene taking the remaining height (min 210-270px phone, 300-430px at 760px, 340-480px at 1024px). Actions are a full-width stack on phone (max 420px) and sit side by side, left-aligned, from 760px.
- **Header:** logo disc and name left, the primary phone number right. Never sticky.
- **Services:** heading then rows on phone; at 1024px a 4fr / 7fr split with rows in two columns (40px column gap).
- **Why / How:** two columns at 1024px (72px gap): heading, lede and benefits left; steps and the Facebook block right. Benefits are always a two-column grid with 24px column gap.
- **Quote:** heading block then form on phone; 5fr / 6fr at 1024px (64px gap).
- **Footer:** stacked on phone; brand and links split left/right from 760px.
- Breakpoints: 400px (tightens header), 760px, 1024px.

### Named Rules
**The First-Screen Rule.** On the first phone screen: the phone number top-right, headline, one-line promise, both quote actions, and the moving scene. No sticky bottom call bar, ever; the header number and the actions carry calling.

## Elevation & Depth

Flat. Depth comes from the hero's vertical gradient (#183466 to navy), the canvas scene's own painted aluminium and shingles, and the alternation of grounds through water seams. Two soft ambient shadows exist and nothing else.

### Shadow Vocabulary
- **Button lift** (`box-shadow: 0 6px 16px -8px rgba(3,10,24,.6)`): filled primary buttons only, a soft pool under the button on navy.
- **Logo disc** (`box-shadow: 0 4px 14px -4px rgba(0,0,0,.5)`): the header logo disc only.

### Named Rules
**The Water-Not-Walls Rule.** Sections are separated by animated water seams (64px phone, 100px at 760px): three sine-driven strokes in Royal, Rain-Light and a mid blue over the next section's fill, paused off-screen and static under reduced motion. Never a straight border or a shadow between sections.

## Shapes

Softly rounded rectangles for things you press or type into, full circles for the logo and row arrows, and hairlines for lists. Buttons round at 14px; fields and chips at 12px. Strokes are 2px on interactive elements, 1px on dividers. No card containers anywhere.

## Components

### Buttons
Big, plain, thumb-sized.
- **Shape:** gently rounded (14px), min height 58px, 26px side padding, 800 18px label, optional 20-22px inline SVG icon at a 10px gap.
- **Primary:** Royal fill with a 2px matching stroke and the button-lift shadow; hover to Pressed Royal; press nudges down 1px. Used for "Get a free quote", the Facebook button and the form submit.
- **Ghost:** transparent with a 2px light-blue stroke (#8fb6f5) and Rain Ink label; hover turns the stroke white over a faint blue wash (rgba(127,176,255,.12)). Only on navy; the "Text us a photo" companion to the primary.
- **Focus:** 3px outline at 3px offset, Wet Leaf on navy, Burnt Leaf on mist. The submit also shows the Burnt Leaf outline on hover.

### Service Rows (signature)
- **Style:** full-width links, 800 20px Slate Ink, min height 64px, hairline Mist Rule above and below. A 42px circular arrow sits at the end with a 2px Mist Rule stroke.
- **Hover / Focus:** the row itself never changes: no background, no outline, no shadow. Only the arrow fills Royal with a white arrow; keyboard focus adds a 3px Royal outline around the arrow.
- Each row links to the quote form and preselects its service chip.

### Benefits and Steps
- **Benefits:** two-column list of 800 20px items, each with a 1px Navy Rule above, 12px vertical padding. No icons, no checkmarks.
- **Steps:** ordered list with the 40px italic Rain-Light numeral in a 44px column; a 20px bold lead line and a dim-ink follow-on line.

### Chips
- **Style:** white fill, 2px Field Steel stroke, 12px radius, min height 46px, 700 16px label. Checkbox chips for services, radio chips for building height.
- **State:** hover or keyboard focus gives a 3px Burnt Leaf outline and stroke. Selected fills Deep Gutter Navy with white text and reveals an amber check glyph.

### Inputs / Fields
- **Style:** white fill, 2px Field Steel stroke, 12px radius, 500 18px text, 14px padding, min height 54px (textarea 110px, vertical resize). Labels 800 18px above; "(optional)" in 500 Dim Slate Ink.
- **Hover / Focus:** 3px Burnt Leaf outline at 1px offset and Burnt Leaf stroke.
- **Error:** Brick stroke and a 700 16px Brick message beneath, written as a plain request.

### Navigation (header)
- Logo disc (46px phone, 42px under 400px, 56px at 1024px) plus 900 italic uppercase name (18 / 16 / 22px). Phone link right: 800 16px (20px at 1024px), tabular numerals, an 18px phone icon in Rain-Light Blue that turns Wet Leaf on hover; icon hidden under 400px. 44px tap height. No menu.

### Gutter Scene (signature)
A canvas eavestrough under slate shingles in rain: leaves (8 autumn colors) pack the trough and water sheets over the lip until a bin is cleared; the pointer (46px reach) pulls leaves loose and the downspout runs. It plays itself with a sweep every 5.5s until first touched. A static CSS gradient still sits beneath for no-JS and reduced motion. Tunables live in its CFG block (leaf density, regrow rate, reach, spring, gravity, rain, self-play cadence, sheet threshold).

### Footer
Navy ground, 72px logo disc, 900 italic uppercase name, both phone numbers and the Facebook link as 44px-tall 700 links (hover Rain-Light), then a dim fact line. Contact lives here and in the header only; no email until one is known.

## Do's and Don'ts

### Do:
- **Do** keep every ground navy or mist; the darkest value is #0c1a33.
- **Do** set every heading 900 italic uppercase with -0.02em tracking and 0.95 line height, and everything else in sentence case.
- **Do** join every navy/mist change with an animated water seam that pauses off-screen and stops under reduced motion.
- **Do** use Royal for every primary action and reserve amber for focus, selection and the selected-chip check.
- **Do** use Burnt Leaf (#b96f14) for focus and hover outlines on mist and Wet Leaf (#e7a23b) on navy.
- **Do** keep tap targets at 44px minimum and buttons at 58px.
- **Do** keep text at 16px minimum.

### Don't:
- **Don't** use black (#000) for any surface or text.
- **Don't** add a sticky or fixed bottom call bar.
- **Don't** put a phone number on the first screen anywhere but top-right of the header.
- **Don't** show an email address anywhere; when one is known it goes in the footer only.
- **Don't** outline, box, shade or fill a service row on hover or focus; only its arrow responds.
- **Don't** wrap lists in cards or add checkmark or icon bullets to benefits.
- **Don't** add eyebrows, kickers or small uppercase labels above headings.
- **Don't** use amber as a fill for buttons, banners or sections.
- **Don't** separate sections with straight borders or shadows.
