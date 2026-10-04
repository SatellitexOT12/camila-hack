---
name: "Camila // acceso comprometido"
description: "Phosphor-green CRT terminal that fakes a breach, hides a birthday greeting inside an easy sudoku, and never dead-ends."
colors:
  phosphor-green: "#00FF41"
  phosphor-pale: "#C8FFD4"
  phosphor-deep: "#0B3D0E"
  phosphor-deep-hover: "#12551f"
  amber-live: "#FFD23F"
  alarm-red: "#FF4646"
  alarm-soft: "#FF8080"
  crt-black: "#000000"
  hairline: "rgba(0,255,65,0.26)"
  hairline-strong: "rgba(0,255,65,0.62)"
typography:
  display:
    fontFamily: "VT323, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "clamp(3rem, 12vw, 6rem)"
    fontWeight: 400
    lineHeight: 0.98
    letterSpacing: "0.02em"
  headline:
    fontFamily: "VT323, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "clamp(2.6rem, 11.5vw, 6rem)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "0.01em"
  subhead:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "clamp(0.95rem, 2.6vw, 1.1rem)"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "11px"
    fontWeight: 400
    letterSpacing: "0.16em"
  console:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "13.5px"
    fontWeight: 400
    lineHeight: 1.6
  console-compact:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "12.5px"
    fontWeight: 400
    lineHeight: 1.6
  sysline:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.55
  meta:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: 1.6
  keypad:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "17px"
    fontWeight: 600
    lineHeight: 1
  keypad-compact:
    fontFamily: "IBM Plex Mono, ui-monospace, 'Cascadia Mono', Consolas, monospace"
    fontSize: "16px"
    fontWeight: 600
    lineHeight: 1
rounded:
  none: "0px"
  dot: "50%"
spacing:
  xs: "6px"
  sm: "10px"
  md: "12px"
  lg: "14px"
  xl: "16px"
  2xl: "24px"
components:
  status-bar:
    backgroundColor: "{colors.crt-black}"
    textColor: "rgba(200,255,212,0.78)"
    typography: "400 11px/1 IBM Plex Mono, uppercase, letter-spacing 0.16em"
    rounded: "{rounded.none}"
    height: "44px"
    padding: "0 16px"
  console-panel:
    backgroundColor: "rgba(0,10,3,0.72)"
    textColor: "rgba(200,255,212,0.9)"
    typography: "400 13.5px/1.6 IBM Plex Mono"
    rounded: "{rounded.none}"
    padding: "14px 16px"
  console-panel-egg:
    backgroundColor: "rgba(0,10,3,0.72)"
    textColor: "rgba(200,255,212,0.62)"
    typography: "400 13.5px/1.6 IBM Plex Mono"
    rounded: "{rounded.none}"
    padding: "14px 16px"
  cell-given:
    backgroundColor: "rgba(0,255,65,0.05)"
    textColor: "{colors.phosphor-pale}"
    typography: "600 calc(var(--cell) * .46)/1 IBM Plex Mono, tabular-nums"
    rounded: "{rounded.none}"
    padding: "0"
  cell-active:
    backgroundColor: "rgba(255,210,63,0.20)"
    textColor: "{colors.amber-live}"
    rounded: "{rounded.none}"
  cell-conflict:
    backgroundColor: "rgba(255,70,70,0.16)"
    textColor: "{colors.alarm-red}"
    rounded: "{rounded.none}"
  pad-key:
    backgroundColor: "rgba(0,255,65,0.05)"
    textColor: "{colors.phosphor-green}"
    typography: "600 17px/1 IBM Plex Mono"
    rounded: "{rounded.none}"
    padding: "0"
  btn-action:
    backgroundColor: "rgba(0,255,65,0.07)"
    textColor: "{colors.phosphor-green}"
    typography: "600 11.5px/1 IBM Plex Mono, uppercase, letter-spacing 0.14em"
    rounded: "{rounded.none}"
    padding: "13px 8px"
  btn-danger:
    backgroundColor: "rgba(255,70,70,0.07)"
    textColor: "{colors.alarm-soft}"
    typography: "600 11.5px/1 IBM Plex Mono, uppercase, letter-spacing 0.14em"
    rounded: "{rounded.none}"
    padding: "13px 8px"
  sys-line:
    backgroundColor: "transparent"
    textColor: "{colors.phosphor-pale}"
    typography: "400 13px/1.55 IBM Plex Mono"
    rounded: "{rounded.none}"
    padding: "10px 0 0"
  meter-tick:
    backgroundColor: "{colors.alarm-red}"
    rounded: "{rounded.none}"
    width: "7px"
    height: "11px"
  reveal-stats:
    backgroundColor: "transparent"
    textColor: "rgba(200,255,212,0.7)"
    typography: "400 12px/1.7 IBM Plex Mono, uppercase, letter-spacing 0.14em"
    rounded: "{rounded.none}"
    padding: "0"
---

# Design System: Camila // acceso comprometido

## Overview

**Creative North Star: "The Compromised CRT Terminal"**

This is a one-file birthday experience dressed as a terminal that has just been breached. The interface is diegetic: a status bar with a pulsing dot and a live clock, a phase label that changes voice as the story moves (`Conectando` → `Intrusión activa` → `Defensa en curso` → `Acceso concedido`), an integrity meter, and a system line that answers every move in Spanish. Nothing floats free of the fiction, and nothing competes with it — there is no navigation, no scroll, and no second screen. Everything the viewer reads sits centered in a single column over a full-viewport canvas of falling `0`/`1` digits.

The material is a CRT: pure black (#000000) is the only backdrop, phosphor green (#00FF41) is the system's life force, and a fixed overlay of 1px scanlines plus a radial vignette sits above the whole page. Depth is made of glow, not shadow — display type and live digits carry `text-shadow` bloom, panels are separated by 1px hairlines, and boxes are drawn with corner brackets rather than fills. Type splits cleanly in two: VT323 (the CRT display face) shouts the two story messages, IBM Plex Mono carries every other string, with system chrome set in uppercase at `.16em` tracking and reading copy left in sentence case.

Confirmed visual rejections: the birthday-card canon (confetti, balloons, party color) is out by thesis; so are soft drop shadows, rounded corners, photography, illustration, icon sets, a third typeface, and any "welcome app" shell. Motion grammar is hardware: a CRT power-on `scaleY` snap, typewriter lines with a blinking block caret, digits that scramble and lock into letters, and — at the end — the sudoku's own digits flying into the shape of the greeting while the rain itself spells `CAMILA` behind it. Under `prefers-reduced-motion: reduce` the rain paints one static frame, all text renders instantly, the chip flight never spawns, and the ghost word stamps once as a static digit field.

**Key Characteristics:**
- Two-font terminal voice: VT323 (`clamp(3rem, 12vw, 6rem)`) for the two shout messages, IBM Plex Mono (15px/1.6) for everything else.
- `#000000` is the only backdrop; separation comes from green-tinted panel alpha (`rgba(0,10,3,.72)`, `rgba(0,8,2,.93)`) and 1px phosphor hairlines (`.26` / `.62` alpha).
- Glow is the only depth cue (`text-shadow`, `0 0 4px → 0 0 16px` phosphor bloom); zero drop shadows, zero radius outside the 7px status dot.
- Amber (#FFD23F) marks exactly one thing — the live cell; red (#FF4646 / #FF8080) marks only conflict, danger, and error.
- A fixed CRT layer (scanlines + vignette, `z-index: 7`, `pointer-events: none`) covers every screen state.
- One screen, one act: rain → typed breach → sudoku → the 81 digits reassemble `¡FELIZ CUMPLEAÑOS, CAMILA!`.
- On reveal the falling rain is clipped into a giant VT323 `CAMILA` watermark in phosphor-deep behind the greeting — the same canvas, not an image.
- Reduced motion collapses every animation to `.01ms` and swaps live canvases/animations for static or instant equivalents.

## Colors

The palette is one hue of green doing four jobs (alive, dead, pale, hairline), guarded by two law-bound accents — amber for the single live cell, red for conflict — over a black that never changes.

### Primary
- **Phosphor Green** (#00FF41): the system's life. Display type, keypad digits, filled cells, prompt glyphs (`>`), rain strokes, focus rings, `::selection` background, the `ok` system line, and the reveal debris chips. It is also the source of both hairline colors.
- **Phosphor Pale** (#C8FFD4): reading text. Body copy (15px), boot console lines at 90% alpha, status bar/plate at 78% alpha, given sudoku digits, and the default system line. Long-form strings are never set in full-strength green.

### Secondary
- **Amber Live** (#FFD23F): reserved to the active cell — 20% background wash, 1px inset ring, amber digit, 10% alpha `text-shadow` glow. It appears nowhere else in the file (grep-verified).

### Tertiary
- **Alarm Red** (#FF4646): conflict and danger only — conflicting cells (16% wash + glow), the `Rendirse` button border, the integrity meter's filled ticks, the status dot, and the noscript box border.
- **Alarm Soft** (#FF8080): the *text* weight of alarm — danger button label, error system lines, noscript copy. Red text that must be read at small sizes uses this, not #FF4646.

### Neutral
- **CRT Black** (#000000): page, status bar, plate, scrollbar track, selection text, and the armed danger button's label.
- **Phosphor Deep** (#0B3D0E): the dead green — scrollbar thumb, the `CAMILA` ghost watermark drawn on the reveal canvas, anything powered down.
- **Phosphor Deep Hover** (#12551f): the warmed step of the dead green — scrollbar thumb hover only.
- **Hairline** (rgba(0,255,65,0.26)): default 1px structure — bar bottom, plate top, cell separators, console frame, keypad key borders, the rule above the system line.
- **Hairline Strong** (rgba(0,255,65,0.62)): emphasized 1px structure — module frame, grid frame, 3×3 box separators, action button borders.

Panel backgrounds are near-black green tints layered over the rain — `rgba(0,10,3,.72)` for the console, `rgba(0,8,2,.93)` for the module, `#010503` for the grid floor — plus green-tinted alpha washes for cell/key states (`rgba(0,255,65,.05/.07/.12/.16)`). These stay as component-level literals; they are not color tokens.

### Named Rules
**The Amber Law.** #FFD23F exists on one element: the currently selected sudoku cell. Not hover, not focus chrome, not headings, not accents. Its scarcity is what makes selection unmistakable.

**The Alarm Rule.** Red means the system is reporting a problem: row/column/box conflicts, danger actions, error lines. It never decorates, and readable red text uses #FF8080 rather than #FF4646.

## Typography

**Display Font:** VT323 (with `ui-monospace, 'Cascadia Mono', Consolas, monospace` fallback) — CSS token `--crt`.
**Body Font:** IBM Plex Mono 400 (same fallback stack) — CSS token `--mono`.
**Label/Mono Font:** IBM Plex Mono 600 for button labels and cell digits (same stack); there is no third face.

**Character:** A hardware pairing: a ragged CRT display face that only ever shouts, and a precise grotesque mono that runs the machine. All three faces are self-hosted woff2 (VT323 400, Plex Mono 400/600) so the page works with the network off.

### Hierarchy
- **Display** (400, `clamp(3rem, 12vw, 6rem)`, line-height .98, letter-spacing .02em, uppercase, phosphor glow): the breach headline `HAS SIDO HACKEADA`. One instance per session.
- **Headline** (400, `clamp(2.6rem, 11.5vw, 6rem)`, line-height 1.02, letter-spacing .01em, uppercase, phosphor glow): the reveal greeting `¡FELIZ CUMPLEAÑOS, CAMILA!`.
- **Subhead** (400, `clamp(.95rem, 2.6vw, 1.1rem)`, line-height 1.6): the prompt line under both messages, prefixed `> ` in phosphor (prefix hides when the line is empty).
- **Body** (400, 15px, line-height 1.6): default page voice in phosphor pale — sentence case, never uppercase.
- **Console** (400, 13.5px, line-height 1.6): boot log lines inside the console panel (including egg replies).
- **Console Compact** (400, 12.5px, line-height 1.6): the same log lines below 420px.
- **System Line** (400, 13px, line-height 1.55): the module's feedback line and the noscript fallback box.
- **Meta** (400, 12px, line-height 1.6): the reveal's closing lines — `.reveal-meta` at `.16em`, `.reveal-stats` at `.14em`/1.7.
- **Keypad** (600, 17px, line-height 1): sudoku digit keys with tabular figures.
- **Keypad Compact** (600, 16px, line-height 1): the same keys below 420px.
- **Label** (400, 11px, letter-spacing .16em, uppercase): status bar, version plate, module header, skip hint. Button labels are 600/11.5px at .14em.

### Named Rules
**The Two-Face Rule.** Two families, two jobs: VT323 renders only the story's shout messages (and the rain canvas glyphs); every other string — chrome, copy, digits, buttons — is IBM Plex Mono.

**The Terminal Voice Rule.** System chrome is uppercase, 11px, tracked `.16em` (buttons `.14em`); human-readable copy stays sentence case at 13–15px. The case split is how the machine and the message stay distinguishable.

## Layout

A single centered column inside a fixed-height frame: status bar (`--bar-h: 44px`, `z-index: 5`) → stage (`flex: 1`, CSS grid, `place-items: center`, `z-index: 2`) → version plate (`min-height: 36px`, `z-index: 5`, `padding-bottom: calc(6px + env(safe-area-inset-bottom))`). Fixed atmosphere layers bracket it: the rain canvas at `z-index: 0`, the CRT overlay at `z-index: 7`, and reveal debris at `z-index: 6`. The CAMILA ghost layer is not a separate DOM layer — it composites inside the rain canvas at `z-index: 0` during the reveal (see Components).

Content widths: `.act` caps at `44rem` (`62rem` for the reveal), the boot console at `34rem`, and the sudoku module at `calc(50px * 9 + 28px)` = 478px. Stage gutters are `20px 12px`, widening to `36px 24px` at ≥760px.

Spacing rhythm (frontmatter steps): `xs 6px` (keypad/action gaps), `sm 10px` (rule under the module header, padding above the system line), `md 12px` (module padding, stage gutter, gap between header and rule), `lg 14px` (console padding, keypad top margin, system line top margin), `xl 16px` (bar/plate inline padding, chrome gaps), `2xl 24px` (desktop stage gutter). Module header is `padding-bottom: 10px; margin-bottom: 12px`; keypad `margin-top: 14px; gap: 6px`; actions `margin-top: 6px; gap: 6px`; console `margin: 0 auto 26px` (34px ≥760px).

Board sizing is fluid, not breakpoint-driven: `--cell: min(calc((100vw - 72px) / 9), 50px)` — cells cap at 50px and shrink with the viewport, with digit size set at `calc(var(--cell) * .46)`. This is what makes 360px-wide phones safe without a dedicated query.

Responsive rules (only two breakpoints ship):
- **≤420px:** chrome tracking tightens to `.12em`, the phase label hides, console padding drops to 12px (copy to 12.5px), module padding to 10px, keypad digits to 16px, action buttons to 11px/.1em with `12px 4px` padding.
- **≥760px:** stage padding opens to `36px 24px`, console margin-bottom to 34px.

Density is one-screen: `body` is `min-height: 100dvh` with `overflow-x: hidden`, no content scroll, no navigation, and bar/plate strings collapse with ellipsis rather than wrapping.

## Elevation & Depth

This system has no drop shadows at all — depth is a hybrid of fixed layer stacking and phosphor bloom. The rain canvas, stage, chrome, debris, and CRT overlay are ordered purely by `z-index`; panels separate from the backdrop by being *nearly* black (`rgba(0,10,3,.72)`, `rgba(0,8,2,.93)`) rather than lighter; and anything that should feel electrified gets `text-shadow` glow. The one `box-shadow` that exists is a zero-blur ring (`0 0 0 1px rgba(0,0,0,.6)`), which is a hard edge, not a soft shadow.

### Shadow Vocabulary
- **Phosphor glow** (`text-shadow: 0 0 4px rgba(0,255,65,.8), 0 0 16px rgba(0,255,65,.42)`): display type, headline, and the `ok` system line. The system's signature bloom.
- **Cell fill glow** (`text-shadow: 0 0 8px rgba(0,255,65,.55)`): digits the player has entered (never givens).
- **Active glow** (`text-shadow: 0 0 10px rgba(255,210,63,.75)` + `box-shadow: inset 0 0 0 1px #FFD23F`): the live cell only.
- **Conflict glow** (`text-shadow: 0 0 9px rgba(255,70,70,.7)`): red cells, paired with a 0.3s shake.
- **Debris glow** (`text-shadow: 0 0 10px rgba(0,255,65,.8)`): flying digit chips during the reveal.
- **Hard ring** (`box-shadow: 0 0 0 1px rgba(0,0,0,.6)`): console panel separation over the rain.

### Named Rules
**The Glow-Only Rule.** If it needs to lift off the page, it glows (`text-shadow`) or it is outlined with a 1px hairline. Soft, blurred `box-shadow` elevation does not exist in this world.

## Shapes

Square-cornered terminal geometry: every element sits at `0px` radius (`rounded.none`), separated by 1px hairlines rather than fills or rounded containers. Recurring silhouettes: the module frame carries two 9px phosphor L-brackets (top-left and bottom-right corner ticks drawn with `::before`/`::after`); the 9×9 grid uses light hairlines between cells with `hairline-strong` separators every third row/column; keypad keys and action buttons are strict rectangles (keypad at `aspect-ratio: 1`); the integrity meter is ten 7×11px solid ticks. No clipping, no masks beyond the CRT gradient overlay, no pills, no chips with radius.

### Named Rules
**The Square Rule.** Every element sits at `0px` radius, separated by 1px hairlines. The single exception in the whole build is the 7px status dot (`border-radius: 50%`) — recorded as the build's one round element, not a general radius allowance. The direction contract asked for "ninguna esquina redondeada"; this dot is the recorded divergence, and `rounded.dot` is keyed to it rather than offered as a generic scale.

## Components

Chrome is diegetic and quiet: it frames the fiction and never asks for attention.

### Status Bar & Plate (header / footer)
- **Shape:** header `44px` tall, footer `min-height: 36px`, both full-bleed on `#000000`, 1px `hairline` rule (bottom / top), inline padding `0 16px`, gap 16px.
- **Typography:** Label treatment — 11px, uppercase, `.16em` tracking, `rgba(200,255,212,.78)`; the phase label switches to phosphor, the clock uses tabular numerals in phosphor pale.
- **States:** the 7px dot pulses (`opacity 1 → .25`, 1s `steps(2)`) and is `#FF4646` during boot/alert/puzzle, flipping to `#00FF41` under `body[data-phase="reveal"]`. Phase labels: `Conectando` / `Intrusión activa` / `Defensa en curso` / `Acceso concedido`. Below 420px the phase label hides.
- **Footer:** `Canal cifrado` left, `0x7F3A // v0.9.4` right, with safe-area bottom padding.

### Console Panel (boot log card)
- **Shape:** left-aligned block, `max-width: 34rem`, centered by auto margins, padding `14px 16px` (12px ≤420px), 1px `hairline` border, background `rgba(0,10,3,.72)` over the rain, hard 1px black ring.
- **Content:** three typed lines at 13.5px in `rgba(200,255,212,.9)`, each ending in a phosphor block caret (`.55em × 1em`, 1s `steps(2)` blink) that disappears once the line is `done`.
- **Behavior:** typing runs at 26ms/char; tap/Enter (or reduced motion) jumps to the finished string.
- **Egg replies:** typing `help`, `hola`, `cumples` or `camila` on a physical keyboard during boot/alert appends a dimmer reply line (`.egg`, `rgba(200,255,212,.62)`) to this panel, typed at 24ms/char through the same mechanism (instant under reduced motion); a rolling 16-char buffer matches word suffixes, only the last four replies are kept, and each reply retires its caret via `done`. Once the puzzle is up, keys belong to the sudoku.

### Alert & Reveal Messages (signature display)
- **Shape:** centered VT323, uppercase, phosphor with the full glow; `.display` at `clamp(3rem,12vw,6rem)`/`.98`, `.greet` at `clamp(2.6rem,11.5vw,6rem)`/`1.02`.
- **Decoder state:** each character is born as a random digit, scrambles every 55ms, then locks into its letter with a `lockPop` (scale 1.22 → 1, 22px bloom, .32s `cubic-bezier(.2,.9,.3,1)`). Words are wrapped `nowrap` so lines break only at spaces.
- **Sub-line:** sentence-case prompt under the message with a `> ` phosphor prefix; the `> pulsa para acelerar` hint (11px, `.16em`) hides once the viewer taps or presses Enter.

### Sudoku Module (game container)
- **Shape:** `max-width: calc(50px * 9 + 28px)`, padding `12px` (10px ≤420px), 1px `hairline-strong` frame on `rgba(0,8,2,.93)`, with 9px phosphor corner brackets top-left and bottom-right.
- **Header:** label treatment (`rgba(200,255,212,.82)`, `.16em`, uppercase) — difficulty left; integrity meter + `Integridad 30 %` right in `#FF4646`, flipping to phosphor in reveal phase.
- **Integrity meter:** ten 7×11px ticks — unfilled `rgba(255,70,70,.18)`, filled `#FF4646`; in reveal phase both states become phosphor tints (`.16` / full). Boot state is 3/10 = `Integridad 30 %`; solving drives it to 10/10 `Integridad 100 %`; surrendering sets 6/10 `Acceso autorizado`.

### Sudoku Cells (the input primitive)
- **Shape:** square at `var(--cell)` (`min((100vw - 72px)/9, 50px)`), transparent background, 1px `hairline` right/bottom separators, `hairline-strong` on the 3×3 box edges, no borders on the outer edge; digits at `600 calc(var(--cell) * .46)/1` mono with `tabular-nums`.
- **States:**
  - *given* — pale digit on `rgba(0,255,65,.05)`, `cursor: default`, no hover, not editable (attempts answer `esa celda está fija, no se puede tocar`).
  - *hover (empty)* — `rgba(0,255,65,.12)` wash.
  - *related* (same row/col/box as active) — `rgba(0,255,65,.07)`; *same digit* — `rgba(0,255,65,.16)`.
  - *active* — the Amber Law state: `rgba(255,210,63,.20)` wash, amber digit, 1px inset amber ring, amber glow.
  - *filled* (player-entered) — phosphor digit with `0 0 8px rgba(0,255,65,.55)` glow; givens never glow.
  - *conflict* — `#FF4646` digit (forced with `!important`), `rgba(255,70,70,.16)` wash, red glow, `shake .3s ease` (±3px).
  - *hint* — 0.9s `hintFlash` from `rgba(0,255,65,.7)` with black digit to transparent.
- **Behavior:** roving-tabindex grid (one tab stop, arrow-key navigation), per-cell Spanish `aria-label` (`fila N, columna N, pista/valor/vacía`), `user-select: none`.

### Keypad
- **Shape:** 9 equal columns, `gap: 6px`, square keys (`aspect-ratio: 1`), 1px `hairline` border on `rgba(0,255,65,.05)`, digits `600 17px` phosphor (16px ≤420px).
- **Remaining count:** a small 11px counter (`<i>`, bottom-right, `rgba(200,255,212,.8)`) shows how many of that digit remain; at zero the key disables — dim `rgba(0,255,65,.12)` border, `rgba(200,255,212,.4)` text, `cursor: not-allowed`.
- **States:** hover lifts to `rgba(0,255,65,.16)` + `hairline-strong`; active presses `translateY(1px)` and inverts to solid phosphor on black (`.14s` color transitions, `.08s` transform).

### Action Buttons
- **Shape:** 1px `hairline-strong` on `rgba(0,255,65,.07)`, phosphor label at `600 11.5px` uppercase `.14em`, padding `13px 8px`, three equal columns (`gap: 6px`), `0px` radius.
- **Hover / active:** background to `rgba(0,255,65,.18)`; press nudges `translateY(1px)` (`.16s` / `.08s` transitions).
- **Danger variant (`Rendirse`):** border `rgba(255,70,70,.55)`, label `#FF8080`, background `rgba(255,70,70,.07)`; hover to `rgba(255,70,70,.18)` + `#FF4646` border.
- **Two-step confirm:** first click swaps the label to `¿Seguro?` and arms the button — solid `#FF4646` on black with a 1s `steps(2)` pulse; it reverts after 3200ms if untouched. Second click surrenders and jumps to the reveal (6/10 meter, `rendición aceptada · el acceso siempre fue tuyo`).
- **Restart:** `> reiniciar sesión` appears only after the reveal completes (padding `14px 22px`, enters with the standard `enter` animation).

### System Line
- **Shape:** 13px/1.55 phosphor-pale text on a 1px `hairline` top rule with `10px` padding-top, `min-height: 3.1em` so messages never shift the layout, prefixed `> ` in phosphor.
- **States:** default pale; `.err` sets `#FF8080` text with a `#FF4646` prefix (conflicts, fixed cells, wrong solutions); `.ok` sets phosphor with the full glow (hints, `defensa superada`, `ACCESO CONCEDIDO`). Messages type in at 16ms/char and are announced via `aria-live="polite"`.

### Reveal Choreography
1. Phase flips to `reveal`: meter and header recolor to phosphor, status dot turns green, rain intensity rises, and the rain canvas starts compositing the CAMILA ghost layer.
2. `ok` system line, 420ms beat, then the sudoku act leaves (`opacity 0`, `translateY(-10px)`, `blur(3px)`, .28s ease) and is hidden.
3. The reveal act enters (`opacity 0 → 1`, `translateY(14px) → 0`, .5s `cubic-bezier(.16,.84,.28,1)`); the greeting decodes with 740ms flight and 52ms per-character stagger.
4. Simultaneously, one debris chip per filled cell launches from its cell center to its letter's center: 19px phosphor digits, `scale 1 → 1.25 → .55`, arc offset `-70px`, 760ms each, 46ms stagger, `cubic-bezier(.22,.72,.24,1)`, removed on finish; the module itself fades down (`translateY(-14px) scale(.97)`, 520ms, 300ms delay).
5. Then the sub-line types, the meta line renders (`// ` prefixed, 12px `.16em`), the stats line fills on a win only (`> ` prefixed, 12px `.14em`, below), and the restart button appears. Both outcomes (solved / surrendered) use identical choreography with different copy — the ending is never gated.

### Reveal Stats Line
- **Character:** the win receipt — a stopwatch and record line that quietly turns the fake hack into a game with a time.
- **Shape:** 12px IBM Plex Mono, `.14em` tracking, uppercase, `rgba(200,255,212,.7)`, `margin: 0 0 26px` closing the reveal act (`.reveal-meta` was rebalanced to `6px 0 6px` to make room), `> ` phosphor prefix that suppresses itself when empty (`:empty::before{content:none}`).
- **Content (win path):** `hackeada en 4m 12s · sin pistas` (or `pistas: N`) `· sin rendirse`, then the record part — `récord: X`, or `¡nuevo récord! (anterior X)` when the stored best is beaten. The stopwatch starts at page load; the solve instant is stamped when the grid closes. The very first solve stores a record silently and adds no fourth part.
- **States:** on surrender the element stays empty and renders nothing (prefix suppressed). The record lives in `localStorage` (`camila-hack-record`) entirely inside `try/catch`, so private mode or `file://` never breaks the ending.

### CAMILA Ghost Layer (canvas)
- **Character:** during the reveal the rain itself spells the name — a deep-green watermark of `CAMILA` behind the greeting with live digits running through the letterforms.
- **Build:** two offscreen canvases sized only on load/resize (no per-frame allocation): a mask draws `CAMILA` in VT323 scaled by `measureText` to ~90% of viewport width (capped at 60% of viewport height), centered at (W/2, H×0.47) in `#0B3D0E`. Each frame the layer paints that shape at 55% alpha, stamps the live digit trail over it, clips with `destination-in`, and blits into the rain canvas. Rain stays intact outside the letters; the DOM greeting always sits above (stage `z-index: 2` over rain `z-index: 0`).
- **Triggers:** the mask recomputes on load, on 150ms-debounced resize, and on `document.fonts.ready` so measurement uses real VT323; drawing runs only while `data-phase="reveal"`. Canvas glyphs are VT323 18px (16px below 560px viewport width).
- **Reduced motion:** there is no loop — `setPhase('reveal')` stamps the mask once (also on resize and `fonts.ready`) with a static random digit field (45% density, `rgba(0,255,65,.8)`) clipped to the letters.

### Motion & Reduced Motion
- **World motion:** CRT power-on (`scaleY .004 → 1` with brightness bloom, .75s `cubic-bezier(.2,.9,.25,1)`), act enter/leave, caret blink, status pulse, CRT breathe (7s `steps(60)` opacity), digit scramble/lock, conflict shake, hint flash, chip flight. Divergence noted: the direction contract imagines the alert block "falling" into the viewport; the build snaps it open CRT-style — the stage does the `scaleY` power-on and acts enter by rising from `translateY(14px)`.
- **`prefers-reduced-motion: reduce`:** every animation and transition is crushed to `.01ms` with one iteration, and `.stage` power-on is disabled. In JS the rain paints a single static frame instead of running the loop, typing and decoding render final text immediately, all waits collapse to 0ms, chip flight plus the module fade are skipped entirely, and the ghost word stamps once as a static digit field. Fast-forward mode (tap/Enter) does the same things on demand, independent of the OS setting.

## Do's and Don'ts

### Do:
- **Do** keep corners at `0px`; the only radius in the system is the 7px status dot (`50%`).
- **Do** draw structure with 1px hairlines — `rgba(0,255,65,.26)` by default, `rgba(0,255,65,.62)` for module/grid frames and 3×3 separators.
- **Do** glow anything electrified with `text-shadow` (standard phosphor bloom: `0 0 4px rgba(0,255,65,.8), 0 0 16px rgba(0,255,65,.42)`).
- **Do** set system chrome in uppercase 11px IBM Plex Mono at `.16em` tracking (buttons `.14em`) and keep reading copy in sentence case at 13–15px.
- **Do** reserve VT323 `clamp(3rem, 12vw, 6rem)` for the two shout messages; everything else is IBM Plex Mono.
- **Do** flag keyboard focus with the global ring: `outline: 2px solid #00FF41; outline-offset: 2px`.
- **Do** build on `#000000` only — panels differentiate themselves with green-tinted alpha, never a lighter surface.
- **Do** honor `prefers-reduced-motion: reduce` with static frames and instant text (and keep tap/Enter fast-forward working).
- **Do** give every interactive state a Spanish system-line answer, and keep the ending reachable by both solving and surrender.

### Don't:
- **Don't** add `border-radius` beyond the 7px status dot — the direction contract bans rounded corners outright.
- **Don't** use soft, blurred drop shadows; depth is glow plus 1px hard edges only.
- **Don't** put `#FFD23F` anywhere except the selected sudoku cell.
- **Don't** use red as decoration — `#FF4646`/`#FF8080` are for conflict, danger, and error only.
- **Don't** introduce a third typeface, photography, illustration, or icon sets; the world's only imagery is the `0`/`1` rain canvas and typographic glyphs (`>`, `//`, `0x7F3A`).
- **Don't** reach for birthday-card devices (confetti, balloons, party palettes) — the thesis explicitly rejects that canon.
- **Don't** add navigation, routes, or content scroll; this is one screen with one act.
- **Don't** drop the CRT layer, the scanlines, or the phase-labeled chrome on new surfaces built in this world — they are the world, not decoration.
