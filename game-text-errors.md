# Game Text Errors

The in-game descriptions are written by hand, not generated from the values the game actually
uses, so some of them state numbers or ranges that testing shows to be wrong.

**These CSVs record measured behaviour, not the game's wording.** Where a description has been
found to be wrong, its cell here is corrected. This file is the record of every such correction,
so a reader who compares a cell against the game text can tell a deliberate correction from a
transcription mistake.

## How to add an entry

One row per corrected cell. Give the file, the row's name, the column, what the game text says,
what the cell now says, and where the measurement is recorded. Only add a row once the behaviour
has actually been measured — a description that merely looks wrong is not an entry.

## Corrections

| File | Row | Column | Game text says | Cell says | Measured in |
|---|---|---|---|---|---|
| `gear/gear_talents.csv` | Perfect Empathic Resolve | `description` | `1-15% if self` | `2.3-16.3% if self` | isac-build-engine `docs/research/talents/empathic-resolve.md` |

## Backfill

Corrections made before this file existed are not listed yet. Add them as they are come across,
following the same rule: a row needs a recorded measurement behind it.
