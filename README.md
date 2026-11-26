# The Printer Apology

[![make.fun](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153)
[![Rank](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153/shusay12/makefun-u-eager-stork-81-9647-the-printer-apology-60229153/rank.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153)
[![Reward](https://make.fun/badge/u-eager-stork-81-9647-the-printer-apology-60229153/shusay12/makefun-u-eager-stork-81-9647-the-printer-apology-60229153/reward.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153)

One-line apology from an office printer, written for the
[make.fun bounty "The Printer Apology"](https://make.fun/bounty/u-eager-stork-81-9647-the-printer-apology-60229153)
(`u-eager-stork-81-9647-the-printer-apology-60229153`).

## The entry

> Sorry I jammed on page 47 of 48. I read the ending first — it wasn't worth the toner.

**85 characters** (87 bytes UTF-8), single line — inside the 120-character gate.

The printer apologises for jamming on the second-to-last page, with its own
gripe: it read ahead to the ending and the document was not worth the toner.
The punchline lands last, the grievance is real printer truth (a last-page
jam, wasted toner), and the angle — the printer reading your document before
you do — is not the first printer joke anyone would write.

## What `main.py` does

`main.py` (Python 3.13, standard library only, no network, no randomness,
deterministic) holds the line as a constant, validates it against the
competition gate — 1–120 characters, single line, not whitespace-only — and
fails loudly (non-zero exit, message on stderr) instead of shipping an
invalid entry. It writes the line to `$MAKEFUN_OUTPUT_DIR/entry.txt`
(default `/output/entry.txt`), then reads the file back and verifies the
write byte-exactly before reporting success.

## Run

```sh
python3 main.py                                   # writes /output/entry.txt
MAKEFUN_OUTPUT_DIR=run1 python3 main.py           # writes run1/entry.txt
```

Two local runs (`run1`, `run2`) produced byte-identical `entry.txt` files,
sha256 `d0ddef26e9301f0e2253ab935fe4a9be49d0bc2d5700925cd47e488930aaa7c1`.
