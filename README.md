# The Pembroke File — a locked-cabinet mystery

A noir mystery played through a filing cabinet. The Pembroke Diamond —
thirty-four carats, blue-white — left the Ashford Museum in three minutes of
dark. The insurance investigator who worked the claim filed nothing for three
weeks and vanished, leaving his case file locked in the cabinet by the window.

Five drawers, five locks, and every answer is written somewhere in the room.
Opening the cabinet means actually reading the case — and the last name in it
was never filed at all.

**Play it:** https://app-field-office.vercel.app

## The rooms

1. **Brass dial** — three figures, all on the insurer's bulletin.
2. **Torn page** — the investigator's reconstruction of the route, torn to
   pieces by somebody who wanted the case closed. Reassemble it to learn which
   four alarms were bypassed.
3. **Jammed card tray** — a sliding-block puzzle (17 moves minimum,
   BFS-verified); freeing the marked canvass card releases the slip the wire
   board wants.
4. **Dead desk lamp** — the investigator left the junction box in pieces so
   nobody could read his desk at night. Rebuild the circuit.
5. **The pencil rubbing** — he wrote the name once, bore down hard, and took
   the sheet. Shade over the desk pad and the impression comes up light out of
   the graphite.

## Build

A single HTML file. No dependencies, no build step, no network calls.
Canvas physics (Verlet chain), Web Audio synthesis, pointer-event puzzles,
`prefers-reduced-motion` support, keyboard paths for every puzzle, and
`localStorage` resume. Both sliding-block boards were generated and
difficulty-verified by breadth-first search before shipping.

Built with [Claude Code](https://claude.com/claude-code).

Plays on phones: the room fits any screen, every puzzle works by touch,
and the footer prints the build revision ("File rev N") so a bug report
can say which version it saw.

The touch pass, for the record: every control answers a tap or a drag,
nothing selects or zooms out from under a finger, and the room sheds its
full-screen atmosphere layers on phones so weak GPUs never buckle.
