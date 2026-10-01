---
name: davinci-resolve-mcp
description: An unofficial landing page set as the edit decision list your conversation would print, on continuous-form green-bar paper.
colors:
  paper: "#fbfcf7"
  green-bar: "#dfecd8"
  tractor-strip: "#eef3ea"
  carbon-ink: "#1b2219"
  faded-ink: "#435140"
  perforation: "#a9bfa3"
  approval-green: "#1d5a28"
  marker-green: "#1d7028"
  marker-blue: "#2457b8"
  marker-red: "#b8322a"
  marker-cyan: "#0d7a8c"
  marker-purple: "#7340ad"
  marker-yellow: "#a37800"
  marker-pink: "#b0367a"
typography:
  display:
    fontFamily: "Archivo, Archivo Narrow, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(3.4rem, 9.5vw, 6rem)"
    fontWeight: 850
    lineHeight: 0.92
    letterSpacing: "-0.02em"
    fontVariation: "'wdth' 62"
  headline:
    fontFamily: "Archivo, Archivo Narrow, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.4rem, 5.6vw, 4.25rem)"
    fontWeight: 850
    lineHeight: 0.92
    letterSpacing: "-0.02em"
    fontVariation: "'wdth' 62"
  numeral:
    fontFamily: "Archivo, Archivo Narrow, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(5rem, 15vw, 10.5rem)"
    fontWeight: 900
    lineHeight: 0.82
    letterSpacing: "-0.03em"
    fontFeature: "'tnum'"
    fontVariation: "'wdth' 62"
  title:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.6rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.01em"
    fontVariation: "'wdth' 75"
  lede:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.1rem, 1.6vw, 1.3rem)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Azeret Mono, ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
    fontSize: "0.75rem"
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: "0.06em"
  event-row:
    fontFamily: "Azeret Mono, ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
    fontSize: "0.74rem"
    fontWeight: 400
    lineHeight: 1.75rem
    fontFeature: "'tnum'"
  code:
    fontFamily: "Azeret Mono, ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
    fontSize: "0.82rem"
    fontWeight: 400
    lineHeight: 1.6
    fontFeature: "'tnum'"
rounded:
  hairline: "2px"
  inline-code: "3px"
spacing:
  line: "1.75rem"
  line-compact: "1.6rem"
  strip: "clamp(14px, 3.2vw, 34px)"
  gutter: "clamp(16px, 4vw, 56px)"
  section: "5.25rem"
  cell: "1.1rem"
components:
  button-go:
    backgroundColor: "{colors.approval-green}"
    textColor: "{colors.paper}"
    typography: "{typography.body}"
    rounded: "{rounded.hairline}"
    padding: "0.95rem 1.25rem"
  button-go-hover:
    backgroundColor: "{colors.carbon-ink}"
    textColor: "{colors.paper}"
  button-plain:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.carbon-ink}"
    typography: "{typography.body}"
    rounded: "{rounded.hairline}"
    padding: "0.95rem 1.25rem"
  button-plain-hover:
    backgroundColor: "{colors.carbon-ink}"
    textColor: "{colors.paper}"
  code-block:
    backgroundColor: "{colors.carbon-ink}"
    textColor: "{colors.paper}"
    typography: "{typography.code}"
    padding: "1rem 1.1rem"
  copy-button:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.carbon-ink}"
    typography: "{typography.label}"
    rounded: "{rounded.hairline}"
    padding: "0.45rem 0.6rem"
  copy-button-done:
    backgroundColor: "{colors.marker-green}"
    textColor: "{colors.paper}"
  tab:
    backgroundColor: "transparent"
    textColor: "{colors.faded-ink}"
    typography: "{typography.label}"
    padding: "0.7rem 0.9rem"
  tab-selected:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.carbon-ink}"
  event-row:
    backgroundColor: "transparent"
    textColor: "{colors.carbon-ink}"
    typography: "{typography.event-row}"
    padding: "0 0.5rem"
  signal-stage-key:
    backgroundColor: "{colors.approval-green}"
    textColor: "{colors.paper}"
    padding: "1.1rem 1.1rem 1.25rem"
---

# Design System: davinci-resolve-mcp

## Overview

**Creative North Star: "The Printed Edit List"**

The whole surface is one continuous sheet of line-printer paper: a near-white page banded with pale green bars, held between two tractor-feed strips punched with sprocket holes, torn into sections along dotted perforations. Content prints onto it the way an edit decision list prints: numbered event rows in monospace, four timecodes, a track, and `*` comment lines that annotate what each event did. Every sentence the visitor's assistant hears becomes one event on that list.

Type is stamped, not set. A heavy condensed grotesk (Archivo at 62% width, weight 850 to 900) carries every headline like a report header punched onto the form; the body is the same family at normal width; every machine fact (tool names, paths, timecodes, labels) is in Azeret Mono with tabular figures. Ink is near-black carbon with a faded second impression; the only chroma comes from DaVinci Resolve's own marker colours, darkened to print on paper, used as small category flags, plus one deep approval green for the action and the key claim.

Density is document-like and rhythmic: everything sits on a 1.75rem printer line pitch, green bars are three lines tall, and sections are three lines apart. The page is flat paper and light-only as built. It rejects the dark developer-tool hero with neon gradients, terminal mock-ups and feature-card grids.

**Key Characteristics:**
- One sheet, two tractor-feed strips, dotted perforations between sections.
- Green-bar banding at a three-line period of the 1.75rem line pitch.
- Condensed heavy grotesk display; monospace for every machine fact.
- Carbon ink plus Resolve marker colours as small category flags only.
- `* LABEL:` comment lines as the native annotation device.
- Motion limited to line-by-line printing and the paper advancing.

## Colors

Carbon ink on banded paper, with Resolve's marker colours used the way markers are used: as small flags that sort things into categories.

### Primary
- **Approval Green** (approval-green): the single filled emphasis colour. Primary button fill, the emphasised half of the hero headline, the stamped install step numerals, the key "inside Resolve" stage of the signal path, and "this project" in the pipeline. Passes 8:1 on paper.

### Tertiary (category flags)
- **Marker Green, Blue, Red, Cyan, Purple, Yellow, Pink** (marker-*): Resolve's timeline marker colours, darkened for paper. Each event row and each tool area is assigned one through a `--c` custom property; it appears as a small square flag, a ruler flag, a hover tint (9% mixed into paper) and the active event number. Marker Green also marks "Yes" and fact bullets; Marker Red marks "No", `* NOTE:` labels and the playhead; Marker Blue is the focus ring.

### Neutral
- **Paper** (paper): the sheet, button-plain fill, table and panel backgrounds, text on inverted blocks.
- **Green Bar** (green-bar): the banding stripe, the AI-replacement table row tint, copy-button hover.
- **Tractor Strip** (tractor-strip): the sprocket-hole margins.
- **Carbon Ink** (carbon-ink): all primary text, 1 to 1.5px structural rules, and the inverted code-block ground.
- **Faded Ink** (faded-ink): secondary text, labels, captions, the EDL header metadata.
- **Perforation** (perforation): dashed and dotted rules, sprocket hole rims, table row dividers. Lines only, never text (1.9:1).

### Named Rules
**The Marker Flag Rule.** Marker colours are flags: small squares, ruler flags, a tint at 9% or less, or bold short labels. They never fill a section or a large surface, and only one marker colour is assigned per event or per tool area.

**The One Green Rule.** Approval Green is the only solid-filled accent. It marks the primary action and the single claim the page exists to make; nothing else competes with it.

## Typography

**Display Font:** Archivo at 62% width (variable `wdth` 62–125, `wght` 400–900), with Archivo Narrow, Helvetica Neue, Arial fallback
**Body Font:** Archivo at 100% width, with Helvetica Neue, Arial fallback
**Label/Mono Font:** Azeret Mono (400/500/700), with ui-monospace, SFMono-Regular, Menlo, Consolas fallback

**Character:** A stamped report header over a printout. The condensed heavy grotesk does the shouting in short declarative lines; the monospace does all the reporting, in tabular figures, exactly as a line printer would.

### Hierarchy
- **Display** (850, clamp(3.4rem, 9.5vw, 6rem), 0.92): the hero headline only, balanced wrap.
- **Headline** (850, clamp(2.4rem, 5.6vw, 4.25rem), 0.92): one per section, written as a full sentence ending in a period.
- **Numeral** (900, clamp(5rem, 15vw, 10.5rem), 0.82): stamped figures: the 155/162 count; step numerals use the same face at 4.25rem (3rem on mobile) in Approval Green.
- **Title** (800, 75% width, 1.6rem, 1): tool-area and install-step headings; limit items use the same face at 1.2rem.
- **Lede** (400, clamp(1.1rem, 1.6vw, 1.3rem), 1.5): the paragraph under each headline.
- **Body** (400, 1rem, 1.6): prose capped at 62ch, pretty wrap.
- **Label** (Azeret Mono 500, 0.75 to 0.78rem, 0.04 to 0.06em, uppercase): EDL header, stage locations, table heads, tabs, code-bar captions.
- **Event row / Code** (Azeret Mono 400, 0.74rem on the line pitch; 0.82rem/1.6 in code blocks, tabular figures): event lists, tool names, paths, commands.

### Named Rules
**The Stamped Header Rule.** Headings are always Archivo condensed (62% or 75% width) at 800 or heavier with tight negative tracking. Never set a headline at normal width or light weight.

**The Machine Fact Rule.** Anything a computer reads or prints (tool names, file paths, timecodes, commands, menu paths, counts in labels) is set in Azeret Mono with tabular figures. Human prose is never set in mono.

## Layout

One centred column (max 1240px) inside the sheet. The sheet's horizontal padding is the tractor strip width (clamp(14px, 3.2vw, 34px)) plus a gutter (clamp(16px, 4vw, 56px)); on mobile the gutter becomes 14px. Vertical rhythm is the printer line pitch (1.75rem, 1.6rem at 640px and below): sections pad three lines top and bottom, section heads sit 1.5 lines above their content, and the green bars repeat every six lines (three on, three off).

The hero is a two-column grid (1fr / 1.15fr): stamped headline, lede, actions and facts left; the live event list right. Below 1000px the hero and the Free vs Studio split collapse to one column and the four-stage signal path becomes two by two; below 640px it becomes a single column, install steps stack their numeral above the body, and the comparison table re-flows into per-row cards with inline labels. The tool index uses CSS columns (3 × 16rem). Event rows keep `white-space: pre` and scroll horizontally inside the list rather than wrapping columns; low-value EDL columns (source timecodes, AX, C) hide on mobile.

### Named Rules
**The Line Pitch Rule.** Vertical spacing is a multiple or simple fraction of the line pitch (0.5, 0.75, 1, 1.5, 3 lines). Content should land on the paper's rhythm, not fight the bars.

**The Perforation Rule.** Sections are separated by a 2px dotted perforation that runs the full width of the sheet, through the gutter to the strips. No other section divider is used.

## Elevation & Depth

None. The page is flat paper; there are no box-shadows anywhere. Depth and grouping come from ink: 1.5px carbon rules to bracket the event list and pipeline, 1px carbon borders around tables, panels and the signal path, dashed perforation-coloured rules for soft subdivision, and inversion (Carbon Ink ground with Paper text) for code blocks, signal wire labels and the console line. The only lift is a 1px `translateY` on button hover and a 4px rise of the active ruler flag.

### Named Rules
**The Flat Paper Rule.** Nothing casts a shadow. To separate, rule a line; to emphasise, invert to carbon or fill with Approval Green.

## Shapes

Square and printed. Corners are 2px at most (buttons, copy button) and 3px on inline code; tables, panels, code blocks, stages and the event list are square-cornered. Recurring silhouettes come from the paper itself: circular sprocket holes in the strips, dashed strip edges, dotted perforations, small square category flags (0.5 to 0.6em), and the pentagon ruler flag (a clipped rectangle with a pointed foot, 9 × 14px) mirroring Resolve's timeline markers. The playhead is a 1.5px red line with a small downward triangle cap.

## Components

### Buttons
Decisive and printed: inked edges, no rounding to speak of.
- **Shape:** near-square (2px), 1.5px solid border.
- **Primary (Go):** Approval Green fill, Paper text, Archivo 700 at 88% width, 0.95rem, padding 0.95rem 1.25rem, optional 1.05em stroked SVG icon leading.
- **Plain:** Paper fill, Carbon Ink border and text.
- **Hover / Focus:** both invert to Carbon Ink with Paper text and rise 1px over 160ms (cubic-bezier(.2,.7,.2,1)); focus is a 2px Marker Blue outline at 3px offset.

### Event List (signature)
The hero's edit decision list. Framed above and below by 1.5px carbon rules; a header line in uppercase label type; a ruler with tick marks, one pentagon flag per event at its record-in position, a red playhead and a timecode readout; then numbered rows: flag square, bold three-digit event number, track, source and record timecodes. Beneath each row a `* SAY:` comment line carries the real prompt in Archivo 600 within curly quotes, and the selected event prints a `* TOOL:` line naming the real MCP tool(s) in the event's marker colour. One event is open at a time (003 on load); selecting tints the row 9% toward its marker colour, raises its ruler flag and moves the playhead. Rows print in on load left to right (clip-path reveal, 380ms, 70ms stagger) and are fully visible without JS or with reduced motion.

### Code Blocks
- **Style:** square, Carbon Ink ground, Paper text, Azeret Mono 0.82rem/1.6, horizontal scroll.
- **Bar:** a `* CMD · <context>` caption in uppercase label type on the left, a Paper copy button on the right that turns Marker Green with "Copied" for 1.8s.
- **Console line:** inline inverted carbon block for the literal output line the user should see.

### Tabs
Uppercase mono tabs on a 1px Carbon Ink baseline; the selected tab gains a Paper fill and a full ink border that joins the panel below. Arrow keys move between tabs.

### Tables
Square 1px carbon frame, mono 0.85rem body, uppercase label heads over a 1px ink rule, dashed perforation dividers between rows. Yes/No cells lead with a small square in Marker Green or Marker Red; rows replaced by local AI take a Green Bar tint and a faded "via" sub-line.

### Signal Path
Four square stages in a 1px ink frame divided by ink rules; each stage lists the thing (mono 700), where it runs (uppercase label) and a short note. Inverted carbon wire labels (MCP, HTTP · localhost, Native API) sit on the dividing line between stages. The stage that makes the claim true is filled Approval Green.

### Notes (`* NOTE:` list)
Limits print as an auto-fit list separated by perforation rules; each item leads with a red mono `* NOTE:` label, a condensed 800 title, and a faded sentence.

## Do's and Don'ts

### Do:
- **Do** keep every section on the same sheet: green-bar banding at three lines of the 1.75rem pitch, tractor strips on both edges, dotted perforations between sections.
- **Do** set headlines in Archivo condensed (62% width, 850) as full declarative sentences, and every machine fact in Azeret Mono with tabular figures.
- **Do** use Approval Green (#1d5a28) for the one primary action and the one key claim per view.
- **Do** assign each event or category exactly one marker colour through `--c` and show it as a flag, square, tint or short bold label.
- **Do** annotate with EDL comment lines (`* SAY:`, `* TOOL:`, `* NOTE:`, `* CMD`) where the content is genuinely a comment on an event, a step or a limit.
- **Do** limit motion to printing (left-to-right line reveals) and the paper advancing, and show everything immediately under reduced motion.

### Don't:
- **Don't** use the dark developer-tool hero: neon gradients, terminal mock-ups or a feature-card grid.
- **Don't** add box-shadows, glows or rounded cards; separate with ink rules and perforations instead.
- **Don't** fill large areas with a marker colour, or use more than one marker colour on a single event or area.
- **Don't** set small text in Marker Yellow (3.9:1 on paper) or Marker Cyan on the green bar (4.1:1); they are flag colours.
- **Don't** use Perforation (#a9bfa3) for text; it is a rule colour.
- **Don't** mimic DaVinci Resolve's logo or UI chrome; its marker colours are borrowed as a print convention, not its branding.
