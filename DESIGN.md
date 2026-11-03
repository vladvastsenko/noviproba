---
version: alpha
name: "Stonemason template by 8B"
description: "Near-black page with large light-grey rounded panels, a tight grotesk, a serif for the inscription, and pale stone green accents for a stonemasonry yard. Free HTML template by 8B, MIT."
colors:
  primary: "#151614"
  secondary: "#555753"
  tertiary: "#d9dcc4"
  neutral: "#e7e7e5"
  surface: "#fafaf8"
  on-surface: "#151614"
  night: "#0e100e"
  muted-dark: "#a2a69d"
  tan: "#b39a7f"
typography:
  headline-display:
    fontFamily: Host Grotesk
    fontSize: 73.6px
    fontWeight: 560
    lineHeight: 0.98
    letterSpacing: -0.045em
  headline-lead:
    fontFamily: Host Grotesk
    fontSize: 23px
    fontWeight: 420
    lineHeight: 1.32
    letterSpacing: -0.012em
  body-lg:
    fontFamily: Host Grotesk
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.55
  label-caps:
    fontFamily: Host Grotesk
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.02
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Host Grotesk
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.3
  button:
    fontFamily: Host Grotesk
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.005em
  inscription:
    fontFamily: Source Serif 4
    fontSize: 144px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0.06em
  quote:
    fontFamily: Source Serif 4
    fontSize: 30px
    fontWeight: 420
    lineHeight: 1.22
    letterSpacing: -0.01em
  wordmark:
    fontFamily: Host Grotesk
    fontSize: 217px
    fontWeight: 560
    lineHeight: 0.9
    letterSpacing: -0.055em
rounded:
  none: 0px
  sm: 6px
  md: 14px
  lg: 18px
  xl: 28px
  full: 999px
spacing:
  gap: 10px
  gutter: 56px
  content-max: 1240px
  wall-max: 1420px
  section-y: 150px
  control-height: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    typography: "{typography.button}"
    rounded: "{rounded.full}"
    padding: 0 22.5px
    height: 48px
  button-accent:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.primary}"
    typography: "{typography.button}"
    rounded: "{rounded.full}"
    padding: 0 22.5px
    height: 48px
  nav-pill:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 4px
  badge:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    height: 28px
  panel:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    rounded: "{rounded.xl}"
  card-trade:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.lg}"
  card-stone:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    rounded: "{rounded.sm}"
    padding: 20px 24px
  input-field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    height: 48px
---

# Stonemason template

## Overview

A one-page site for a stonemasonry yard that repairs old buildings, cuts new stone and carves letters. The idea is a dark workshop floor with big pale slabs laid on it: light-grey rounded panels float on a near-black page, and the stone, the team and the jobs sit on them like finished work on a banker. The mood is calm and exact, closer to a heritage trade than a studio. Stone photography does the colouring, so the interface stays grey, with one pale stone green for the main actions and a drawn mark as the signature.

## Colors

- Ink `#151614` (primary): text on light panels, the dark buttons and the pill that holds Menu and Book a site visit.
- Grey `#555753` (secondary): lead paragraphs, labels, step text and job detail lines on light panels.
- Stone green `#d9dcc4` (tertiary): the only accent. Filled buttons, the Menu button, mason marks, lettering prices, the inscription once cut, the second contact heading line, the fill that sweeps across a dark button on hover.
- Panel grey `#e7e7e5` (neutral): the large rounded panels, the logo and call pills, the stone cards, and body text on the dark sections.
- Paper `#fafaf8` (surface): trade cards, badges, the lime comparison card, the frosted quote panes and form field backgrounds.
- Night `#0e100e`: the page ground, the opening, the full-screen menu and the shade over the clients photo.
- Muted `#a2a69d` (muted-dark): secondary text and hairlines on dark sections, and the pale colour the inscription starts from.
- Tan `#b39a7f`: only the three icons under the opening text and the mark on the process photo.

## Typography

Host Grotesk, one variable font, carries everything except the inscription and the quotes. Headings are medium weight (560) at huge sizes with very tight tracking, which keeps long phrases like "Five stones on the banker this year" compact. Small headings (stone names, mason names, job titles) are 15px bold uppercase; the process step titles use the same style at 20 to 28px. Labels are 13px medium, body text is 17px regular. Sizes use `clamp()`: the display size runs from 36px on a phone to about 74px.

Source Serif 4, also variable, appears twice. The three-line inscription is uppercase with wide tracking at up to 144px, and its weight is animated from 250 to 600 on scroll. The three client quotes are set at about 30px, weight 420. Keep the serif off headings and buttons.

## Layout

Content sits in a 1240px column with a gutter that grows to 56px. Light panels have 28px corners and a 10px margin, so the near-black ground shows as a thin frame between them. Sections alternate: panels for trades, process, recent work, lime and questions; open dark sections for the opening, stones, masons, lettering, clients and contact. Most sections put the heading in a narrower column beside the content, a 7 to 5 or 4 to 7 split. The stones form a wall up to 1420px wide: each row has a photo and a light card, and the column widths change from row to row so the courses look laid, not tabled.

At 760px and below, two-column grids become one column, the stone photos shorten to 110px strips above their cards, the process steps become separate cards, and the nav keeps the mark, Menu, Book a site visit and an arrow button; the name and call label are visually hidden.

## Elevation & Depth

One shadow exists: `0 24px 60px -28px` in near-black at 45% opacity, under the trade cards, the frosted panes and the stacked process cards on phones. Depth otherwise comes from overlap. Trade panels stick and cover each other, quote panes rise over the clients photo at different speeds, and the quote panes and form are frosted glass: a translucent paper fill with a 22px backdrop blur.

## Shapes

Corners come in four sizes: 28px for panels, 18px for cards, photos and the process frame, 14px for form fields, and 6px for the stone courses, which are the squarest thing on the page. Buttons, badges and the two nav pills are fully round. Icon buttons are circles. Everything drawn is a thin straight stroke on a 48 unit grid: the cross mark, the plus, the job dashes and the seven mason marks, each a few straight segments with square caps and mitred joins, like a mark cut with a chisel.

## Components

- `button-primary`: the dark pill used for Send to the yard. On hover two diagonal slices of stone green slide in from opposite corners and meet.
- `button-accent`: the stone green pill used for Book a site visit and Commission an inscription, with paper-coloured slices on hover.
- `nav-pill`: the dark capsule holding the green Menu button and the Book a site visit link.
- `badge`: 28px paper capsule on photos and job cards.
- `card-trade`: paper card with a photo half and a text half, four ruled job lines and a text link.
- `card-stone`: the light card beside a stone photo, with name, type and place, and a sentence.
- `input-field`: 48px high translucent paper field with a thin ink border at 30% opacity.

## Motion

The page loads GSAP, ScrollTrigger, SplitText and Lenis. Lenis smooths scrolling (lerp 0.075) and the scenes use scrubbed scroll timelines. The one idea is stone being worked as you scroll: things start rough, offset or pale and arrive finished.

- Opening: on load the heading rises out of a clip in one second, the lead, buttons and facts fade up at 0.12, 0.22 and 0.32 seconds, and the slab photo settles. Nothing moves on scroll.
- Headings: lines rise from a mask in 1 second with a 0.09 second stagger when they reach 88% of the viewport.
- Trades: each card sticks and the next slides over it; the covered card shrinks to 90% and darkens, the arriving photo settles from 118%.
- Stones: rows slide in sideways, photo and card from opposite sides, and the photo shrinks from 130%.
- Process: the photo frame is cut from a rough outline to a sawn square, a moulded profile and the full block, and the mark draws at the end. The step in view gets full opacity, the others 40% on desktop.
- Masons and footer: marks draw stroke by stroke in 0.7 seconds.
- Recent work: the stage pins and the four cards slide sideways, each photo opening from a cropped frame (cut 42% in from the left) to its full size.
- Lettering: the pinned inscription gets two guide lines per row, then its letters go from thin and pale to heavy and green, one row after another.
- Clients: the wall drifts and zooms out while the panes climb at three different speeds and straighten.
- Contact: the two heading lines slide in from opposite sides; the quarry photo behind the form settles.

With reduced motion the entrance and scroll animations and Lenis are not started: trades and process read as plain content and recent work is a sideways-scrolling row. The navigation bar still hides on scroll and button hover fills still run.

## Do's and Don'ts

- Do keep the stone green as the single accent; use tan only for small drawn marks.
- Do keep the serif for the inscription and quotes, and the grotesk for everything else.
- Do keep panels at 28px and stone courses at 6px.
- Do draw every mark as straight path strokes on the 48 unit grid so the cut effect can draw it.
- Don't add a second accent colour, gradients on buttons or coloured shadows.
- Don't use stock icon sets, emoji or round avatars; the marks are the iconography.
- Don't switch the dark sections to light backgrounds; the near-black ground is what makes the panels read as slabs.
