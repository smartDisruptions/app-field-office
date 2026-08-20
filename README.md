# Field Office — an escape-room résumé

An interactive résumé played as an escape room. A locked filing cabinet, five
drawers, five locks — and every answer is written somewhere in the room. Solving
the cabinet means actually reading the file.

**Play it:** https://app-field-office.vercel.app

## The rooms

1. **Brass dial** — three numbers, all on the memo above the cabinet.
2. **Torn page** — drawer two's sheet comes back in twelve pieces; reassemble it
   to read the answer to the switch-bank lock.
3. **Jammed card tray** — a sliding-block puzzle (17 moves minimum, BFS-verified);
   freeing the red card releases the filing slip the wire board wants.
4. **Dead desk lamp** — turn the conduit in the junction box until the live line
   reaches the lamp; only then can the desk pad be seen.
5. **The pencil rubbing** — the last word isn't written anywhere. Shade over the
   desk pad and it comes up light out of the graphite.

## Build

A single HTML file. No dependencies, no build step, no network calls.
Canvas physics (Verlet chain), Web Audio synthesis, pointer-event puzzles,
`prefers-reduced-motion` support, keyboard paths for every puzzle, and
`localStorage` resume.

Built with [Claude Code](https://claude.com/claude-code) — this game is itself
an exhibit of the workflow it describes.
