# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

static HTML/CSS/JS (chosen by the user: single-page, no dependencies, openable by double-click or deployable to any free static host)

## Users

Camila, the recipient: a friend opening a link sent to her on her birthday, most likely on her phone, curious and unsuspecting. The sender (a friend) is a secondary audience who will look at the result once before sharing.

## Product Purpose

A one-shot celebratory web experience that surprises Camila on her birthday. Success: she plays through it to the end and reads the birthday message. The experience must be self-contained, require no account, no backend, and no network calls.

## Positioning

A playful fake "hack" narrative that turns into a gift: the page pretends to hack her, challenges her with a sudoku as the "defense", and the solved sudoku itself becomes the birthday greeting. The mechanism (sudoku numbers resolving into the message) is the whole idea and cannot be copied by a generic greetings card.

## Operating Context

Opened from a shared link on a phone first, desktop second. One session, a few minutes long. No navigation, no other pages.

## Capabilities and Constraints

- Phase 1: falling matrix-style 0/1 animation on entry, a few seconds long.
- Phase 2: message "Has sido hackeada" challenges her to solve a sudoku to stop the hack.
- Phase 3: an easy sudoku she can actually solve (givens chosen so a casual player finishes).
- Phase 4: on solving it, an animation using the sudoku's numbers resolves into "¡Feliz cumpleaños, Camila!".
- All text in Spanish (tuteo/español neutro).
- Fully client-side, single page, offline-capable, no dependencies beyond optional CDN-free code.
- Mobile-first and touch-usable; keyboard entry for desktop.
- Must never dead-end: if the sudoku is too hard there is an escape hatch (skip/reveal) so the message is always reachable.

## Brand Commitments

Binding from the brief: hacker/matrix aesthetic for the opening; the named recipient is **Camila**; the final message is "¡Feliz cumpleaños, Camila!". No extra personal message was provided beyond the name.

## Evidence on Hand

No assets, photos, or copy supplied. The name "Camila" is the only real content given; everything else (sudoku grid, terminal copy, animation text) is authored here and contains no factual claims.

## Product Principles

1. The surprise is the product: never reveal the birthday ending before the sudoku is solved.
2. The puzzle must be winnable by a casual player — easy givens, clear feedback, no lockout.
3. One continuous narrative, no pages, no dead ends.
4. Everything ships in the site's own files; it works with the network off.

## Accessibility & Inclusion

Keyboard-playable sudoku, sufficient contrast on the terminal text, respects prefers-reduced-motion (skip or shorten the falling-rain and number animations), works at 390px width.
