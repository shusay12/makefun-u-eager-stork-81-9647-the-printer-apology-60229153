# Build report — The Printer Apology

Competition: `u-eager-stork-81-9647-the-printer-apology-60229153` — "The Printer Apology" ($2).
Entry deadline: 2026-11-26T14:55:00Z (21:55 WIB). Built 2026-11-26 ~15:00 WIB, well inside the window.

## Chosen line

> Sorry I jammed on page 47 of 48. I read the ending first — it wasn't worth the toner.

- **85 characters**, 87 bytes UTF-8, single line, no trailing newline.
- `entry.txt` sha256: `d0ddef26e9301f0e2253ab935fe4a9be49d0bc2d5700925cd47e488930aaa7c1`
  (two local runs, `run1` and `run2`, byte-identical).

## Why it fits the judge brief (criteria in the brief's order)

1. **Genuine apology, printer's own gripes** — opens with a real apology
   ("Sorry I jammed...") and the gripe is the printer's: it had to print a
   document that was not worth its toner.
2. **The laugh, punch at the end** — the joke turns on the printer reading
   ahead to the ending; the punchline ("it wasn't worth the toner") is the
   last clause, so the laugh lands on first read, at the end.
3. **Printer truth** — a jam on the second-to-last page and wasted toner are
   things a printer would actually suffer; "page 47 of 48" is the most
   annoying possible jam.
4. **Freshness** — the printer reading your document before you do and
   judging it is not the first joke anyone writes about a printer.
5. **Economy** — 85 of 120 characters; every word earns its place. The short
   text also helps the byte-count tie-break.

No text addressed to the judge; no cliché ("out of toner", "turn me off and
on again", "I ate your homework").

## Candidates considered

| # | Line (chars) | Verdict |
|---|--------------|---------|
| 1 | Sorry I jammed on page 47 of 48. I read the ending first — it wasn't worth the toner. (85) | **Chosen** — apology + gripe, punch last, fresh angle, real printer truth, tight. |
| 2 | Sorry for the jam — you fed me the cheapest paper, then acted shocked when I choked. (84) | Rejected — "choked" repeats the jam; punch is a shrug, not a joke. |
| 3 | Sorry I jammed. You keep feeding me damp paper and staples, then swear at me like I chose this life. (100) | Rejected — decent victim punch, but it reads as a complaint list; the joke is thinner and the line is 15 chars longer for no gain. |
| 4 | Sorry I ate your report. In my defence, it was printed on the cheapest paper money can buy. (91) | Rejected — "the printer ate my report" is the first printer joke anyone writes; fails freshness (criterion 4). |
| 5 | Sorry I printed 47 copies of your typo — you clicked print, I only obey. (72) | Rejected — funny, but the printer's own gripe is missing (criterion 1); it blames the user rather than apologising with a grievance. |

## Verification

- `main.py` validates the gate (1–120 chars, single line, non-blank) and
  fails loudly instead of shipping an invalid entry; it verifies the write
  byte-exactly by reading `entry.txt` back and comparing.
- Two runs (`MAKEFUN_OUTPUT_DIR=run1` / `run2`) produced byte-identical
  files (`cmp` clean), sha256 as above.
- No local grade exists for this bounty — the server grades via the AI judge
  (pairwise, blind rounds). Nothing here presents a practice score as a final.
