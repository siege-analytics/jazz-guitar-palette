# Jazz Guitar Palette for MuseScore

A systematic library of moveable jazz guitar chord voicings for MuseScore Studio, organised for chord melody, fingerstyle solo, and comping/vocal contexts across six and seven string guitar.

## Background

This palette grew out of work on chord melody arrangements using Martin Taylor's *Complete Jazz Guitar Method* and Dirk Laukens' *Jazz Guitar Chord Dictionary* as primary references. The goal is a reusable, transposable voicing library that travels across tunes and keys rather than a tune-specific chord sheet.

The palette is documented on [Learning Jazz From The Masters](https://learningjazzguitar.substack.com).

## How to use

### Installing the palette

1. Download the `.mpal` file for the palette you want from the `palettes/` directory
2. Open MuseScore Studio
3. Right-click any palette name in the Palettes panel
4. Select **Load palette** and navigate to the downloaded `.mpal` file

### Using the voicings

All shapes are stored at a reference position (typically root on A string, fret 3 = C). To use in a different key:

1. Place the fretboard diagram in your score
2. Open the Properties panel (F8)
3. Change the **Fret number** to match your target key

Use the fret reference table below to find the correct fret number for any root note on any string.

### Fret reference

| Note | E str (6) | A str (5) | D str (4) | G str (3) | B str (2) | e str (1) |
|------|-----------|-----------|-----------|-----------|-----------|-----------|
| C    | 8         | 3         | 10        | 5         | 1         | 8         |
| Db   | 9         | 4         | 11        | 6         | 2         | 9         |
| D    | 10        | 5         | 12        | 7         | 3         | 10        |
| Eb   | 11        | 6         | 1         | 8         | 4         | 11        |
| E    | 12        | 7         | 2         | 9         | 5         | 12        |
| F    | 1         | 8         | 3         | 10        | 6         | 1         |
| F#   | 2         | 9         | 4         | 11        | 7         | 2         |
| G    | 3         | 10        | 5         | 12        | 8         | 3         |
| Ab   | 4         | 11        | 6         | 1         | 9         | 4         |
| A    | 5         | 12        | 7         | 2         | 10        | 5         |
| Bb   | 6         | 1         | 8         | 3         | 11        | 6         |
| B    | 7         | 2         | 9         | 4         | 12        | 7         |

## Palette architecture

Palettes are organised along two axes: **texture** (is the melody on the guitar or in the voice?) and **string count** (six or seven string).

### Naming convention

Each palette is named `[context][strings] — [voicing type]`:

- `CM6` = Chord Melody, 6-string
- `CM7` = Chord Melody, 7-string (Van Eps tuning: low A)
- `CV6` = Comping/Vocal, 6-string
- `CV7` = Comping/Vocal, 7-string

### Chord Melody / Fingerstyle (melody on the guitar)

The melody note is a hard constraint — voicings are chosen to place the correct melody note on top. Follows the methodology in Martin Taylor's *Complete Jazz Guitar Method*.

| Palette name | Contents |
|---|---|
| `CM6 — Shell` | 1-3-7 and 1-7-3, E-string and A-string root |
| `CM6 — Drop 2` | maj7, dom7, m7, m7b5 — A-string and D-string bass |
| `CM6 — Drop 3` | maj7, dom7, m7, m7b5 — E-string and A-string bass |
| `CM6 — Extended` | maj6, maj6/9, maj9, dom9, dom13, m9, m11 |
| `CM6 — Altered` | dom7b9, dom7#9, dom7b13, dom7#11, 7b5b9, 7b5#9, 7#5b9, 7#5#9 |
| `CM6 — Quartal` | Quartal voicings, string sets 2-3-4-5 and 1-2-3-4 |
| `CM7 — Shell` | 7-string versions, low A available as bass note |
| `CM7 — Drop 2` | 7-string versions |
| `CM7 — Drop 3` | 7-string versions |
| `CM7 — Extended` | 7-string versions |
| `CM7 — Altered` | 7-string versions |
| `CM7 — Quartal` | 7-string versions |

### Comping / Vocal (melody in the voice)

The guitar is freed from melody note constraints. Voicing choices prioritise harmonic colour, voice leading, and space above the chord for a vocal line.

| Palette name | Contents |
|---|---|
| `CV6 — Shell` | 1-3-7 and 1-7-3, E-string and A-string root |
| `CV6 — Drop 2` | maj7, dom7, m7, m7b5 — A-string and D-string bass |
| `CV6 — Drop 3` | maj7, dom7, m7, m7b5 — E-string and A-string bass |
| `CV6 — Extended` | maj6, maj6/9, maj9, dom9, dom13, m9, m11 |
| `CV6 — Altered` | dom7b9, dom7#9, dom7b13, dom7#11, 7b5b9, 7b5#9, 7#5b9, 7#5#9 |
| `CV6 — Quartal` | Quartal voicings, string sets 2-3-4-5 and 1-2-3-4 |
| `CV7 — Shell` | 7-string versions |
| `CV7 — Drop 2` | 7-string versions |
| `CV7 — Drop 3` | 7-string versions |
| `CV7 — Extended` | 7-string versions |
| `CV7 — Altered` | 7-string versions |
| `CV7 — Quartal` | 7-string versions |

## CAGED position reference

Each voicing type corresponds to a CAGED position, which tells you where on the neck the shape lives relative to the root note.

| CAGED shape | Root string | Voicing type | String set | Notes |
|---|---|---|---|---|
| E shape | 6th string | Drop 3 | 6-4-3-2 | Lower register |
| A shape | 5th string | Drop 2 | 5-4-3-2 | Core chord melody voicing |
| A shape | 5th string | Drop 3 | 5-4-3-1 | Melody on high e |
| D shape | 4th string | Drop 2 | 4-3-2-1 | High position chord melody |
| D shape | 4th string | Shell | 4-3-2 | 3-note guide tone chord |

## Build status

| Palette | Status |
|---|---|
| CM6 — Shell | 🔲 Not started |
| CM6 — Drop 2 | 🔲 Not started |
| CM6 — Drop 3 | 🔲 Not started |
| CM6 — Extended | 🔲 Not started |
| CM6 — Altered | 🔲 Not started |
| CM6 — Quartal | 🔲 Not started |
| CM7 — Shell | 🔲 Not started |
| CM7 — Drop 2 | 🔲 Not started |
| CM7 — Drop 3 | 🔲 Not started |
| CM7 — Extended | 🔲 Not started |
| CM7 — Altered | 🔲 Not started |
| CM7 — Quartal | 🔲 Not started |
| CV6 — Shell | 🔲 Not started |
| CV6 — Drop 2 | 🔲 Not started |
| CV6 — Drop 3 | 🔲 Not started |
| CV6 — Extended | 🔲 Not started |
| CV6 — Altered | 🔲 Not started |
| CV6 — Quartal | 🔲 Not started |
| CV7 — Shell | 🔲 Not started |
| CV7 — Drop 2 | 🔲 Not started |
| CV7 — Drop 3 | 🔲 Not started |
| CV7 — Extended | 🔲 Not started |
| CV7 — Altered | 🔲 Not started |
| CV7 — Quartal | 🔲 Not started |

## References

- Taylor, Martin. *Complete Jazz Guitar Method*. Alfred Music.
- Laukens, Dirk. *Jazz Guitar Chord Dictionary*. jazzguitar.be.
- Greene, Ted. *Chord Chemistry*. Alfred Music.

## License

Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to use, share, and adapt this material for any purpose, provided you credit **Dheeraj Chand** and link to this repository.
