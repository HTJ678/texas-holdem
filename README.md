# Texas Hold'em 🎴

A single-file Texas Hold'em game that runs entirely in the browser. No build step, no server, no dependencies, no network requests.

Play against 5 AI opponents with different personalities.

**Play online:** https://htj678.github.io/texas-holdem/

## Features

- **1 human vs 5 AI bots** — each bot has its own tightness / aggression / bluff tendency / IQ profile
- **4 difficulty levels** — Easy / Medium / Hard / Hell (Hell unlocks after clearing Hard)
- **Full hand engine** — blinds, preflop → flop → turn → river, betting rounds, all-in and showdown
- **Showdown panel** — when a hand ends, every remaining player's hole cards and hand type are listed, with the winner marked
- **Procedural background music** — generated live with the Web Audio API (no audio files), toggle with the ♪ button
- **Bilingual** — English by default; switch to 中文 with the top-left button (your choice is remembered)
- **Mobile friendly** — landscape recommended; works offline once opened

## Controls

| Button | What it does |
|---|---|
| 中文 / EN | switch language |
| ♪ | toggle background music |
| Fold / Check / Call / Raise | your action when it's your turn |
| Next Hand | deal the next hand |

## Run it

Open `index.html` in any modern browser. That's it.

## Changelog

### v1.2
**Added**
- Background music: procedurally generated with the Web Audio API (no external files). Four-bar loop at 72 BPM; three chords rising, resolving back to the first on the fourth bar. Toggle with ♪.
- Showdown panel: when a hand is decided, it lists every non-folded player's hole cards and hand type and marks the winner. The bust / victory overlay now waits 2.2 seconds so you can read it first.

**Fixed**
- Language toggle overlapped the difficulty badge.
- Your own hole cards were clipped off the bottom edge in landscape; they now sit on the table, above your name.
- On narrow screens the showdown panel overflowed the right edge.

**Changed**
- Default language is now English. Switch to 中文 from the top-left button; the choice is remembered.

### v1.0
- Initial release: 4 difficulty levels, 5 AI opponents with individual profiles, blinds, betting rounds, all-in, showdown, sound effects.

## Roadmap

- More sound effects (deal, raise, all-in, win/lose stings)
- Optional setting: reveal or hide hands at the end of a hand
- More music sections / a few variations of the loop
- Keyboard shortcuts for actions

## Notes

- Pure vanilla JavaScript + CSS. Everything lives in one file.
- No accounts, no telemetry, no external requests.

## License

MIT
