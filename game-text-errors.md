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

## Where leads come from

A community-maintained guide collects wrong in-game texts and is a useful place to look for
candidates:
<https://docs.google.com/document/d/1zmMtU8JWUXNIObhxst__CYguFgfZ1288mPodyqs2LTE/edit>

It is a lead source, not a source of truth. Nothing from it becomes a row above until we have
measured the behaviour ourselves.

## This list is never complete

Treat it as a living record, never as the full set of wrong descriptions. Two reasons it cannot be
complete:

- Corrections made before this file existed leave no trace that can be recovered. The file history
  shows only what a cell said here, never what the game said, so an old edit could equally be a
  correction, a transcription fix, or a change the game itself made in a patch. A cell that was
  authored correct from the start leaves no trace at all.
- Nobody has checked every description against measured behaviour, and no source that lists these
  errors is complete either.

So entries arrive one at a time, as testing turns one up or as somebody recalls one. A row still
needs a recorded measurement behind it — a description that merely looks wrong is not an entry.
