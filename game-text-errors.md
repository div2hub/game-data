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
| gear/brand_sets.csv | Legatus S.p.A | 1pc_bonus | stat:magazine-size:15% | stat:swap-speed:30% | in-game inspection |
| gear/brand_sets.csv | Legatus S.p.A | 2pc_bonus | stat:smg-damage:24% | stat:optimal-range:70% | in-game inspection |
| gear/brand_sets.csv | Legatus S.p.A | 3pc_bonus | stat:optimal-range:105% | stat:weapon-damage:15% | in-game inspection |
| gear/brand_sets.csv | Habsburg Guard | 2pc_bonus | stat:marksman-rifle-damage:24% | stat:marksman-rifle-damage:20% | in-game inspection |
| gear/brand_sets.csv | Airaldi Holdings | 1pc_bonus | stat:marksman-rifle-damage:12% | stat:marksman-rifle-damage:10% | in-game inspection |
| gear/brand_sets.csv | Royal Works | 2pc_bonus | stat:lmg-damage:24% | stat:lmg-damage:32% | in-game inspection |
| gear/brand_sets.csv | Lengmo | 2pc_bonus | stat:lmg-damage:24% | stat:lmg-damage:20% | in-game inspection |
| gear/brand_sets.csv | Douglas & Harding | 1pc_bonus | stat:pistol-damage:24% | stat:pistol-damage:20% | in-game inspection |
| gear/brand_sets.csv | Badger Tuff | 1pc_bonus | stat:shotgun-damage:12% | stat:shotgun-damage:10% | in-game inspection |
| gear/brand_sets.csv | Fenris Group AB | 1pc_bonus | stat:assault-rifle-damage:12% | stat:assault-rifle-damage:10% | in-game inspection |
| gear/brand_sets.csv | Overlord Armaments | 1pc_bonus | stat:rifle-damage:12% | stat:rifle-damage:10% | in-game inspection |
| gear/brand_sets.csv | Petrov Defense Group | 1pc_bonus | stat:lmg-damage:12% | stat:lmg-damage:10% | in-game inspection |
| gear/brand_sets.csv | Sokolov Concern | 1pc_bonus | stat:smg-damage:12% | stat:smg-damage:10% | in-game inspection |
| gear/brand_sets.csv | Unit Alloys | 2pc_bonus | stat:assault-rifle-damage:24% | stat:assault-rifle-damage:20% | in-game inspection |
| gear/brand_sets.csv | Ceska Vyroba s.r.o. | 2pc_bonus | stat:shotgun-damage:24% | stat:hazard-protection:20% | in-game inspection |
| gear/brand_sets.csv | Urban Lookout | 2pc_bonus | stat:marksman-rifle-damage:24% | stat:marksman-rifle-damage:20% | in-game inspection |
| gear/brand_sets.csv | Zwiadowka Sp. z o.o. | 2pc_bonus | stat:rifle-damage:24% | stat:rifle-damage:20% | in-game inspection |
| gear/brand_sets.csv | Imminence Armaments | 2pc_bonus | stat:pistol-damage:48% | stat:pistol-damage:60% | in-game inspection |
| gear/brand_sets.csv | Imminence Armaments | 1pc_bonus | stat:weapon-damage:6% | stat:weapon-damage:5% | in-game inspection |
| gear/brand_sets.csv | Walker, Harris & Co. | 1pc_bonus | stat:weapon-damage:6% | stat:weapon-damage:5% | in-game inspection |
| `gear/gear_talents.csv` | Perfect Empathic Resolve | `description` | `1-15% if self` | `2.3-16.3% if self` | isac-build-engine `docs/research/talents/empathic-resolve.md` |
| `gear/gear_talents.csv` | Alternating Current | `description` | `stack of 3% skill damage` | `stack of 2.5% skill damage` | isac-build-engine `docs/research/talents/alternating-current.md` |
| `gear/gear_talents.csv` | Intimidate | `description` | `increases weapon damage` | `amplifies weapon damage` | isac-build-engine `docs/research/talents/intimidate.md` |
| `gear/gear_talents.csv` | Perfect Intimidate | `description` | `increases weapon damage` | `amplifies weapon damage` | isac-build-engine `docs/research/talents/intimidate.md` |
| `gear/gear_talents.csv` | Heartstopper | `description` | `+1.1% weapon damage` | `+1.1% amplified weapon damage` | isac-build-engine `docs/research/talents/heartstopper.md` |
| `gear/gear_talents.csv` | Symphony | `description` | `all bonuses are multiplied by 2` | `all bonuses are multiplied by 1.5` | isac-build-engine `docs/research/talents/symphony.md` |
| `gear/gear_talents.csv` | Signature Moves | `description` | `+50% Weapon Damage` | `+50% Amplified Weapon Damage` | isac-build-engine `docs/research/talents/signature-moves.md` |
| `gear/gear_talents.csv` | Point of Honor | `description` | `from 4% to 7%` | `from 4% to 7.2%` | community testing; no recorded measurement |

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
