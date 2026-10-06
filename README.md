# LalaNote Open Music

3,334 scores of classical music and well-known tunes, as MusicXML (`.mxl`) files. They are the score library of the
[LalaNote](https://github.com/mylovejs2/LalaNote) score editor, and anyone may use them.

- `scores/<Composer>/<title>--<id>.mxl` — the scores
- `catalog.json` — one entry per score: title, composer, file, number of staves, parts, measures and pages, licence,
  and `lyrics: true` when the score has sung words. The few scores that do not come from PDMX are marked
  `own: true` and name their edition in `credit`

## Where the scores come from

All but nineteen of the files come from **PDMX**, a dataset of public-domain MusicXML scores collected from MuseScore.com:

> Phillip Long, Zachary Novack, Taylor Berg-Kirkpatrick, Julian McAuley.
> *PDMX: A Large-Scale Public Domain MusicXML Dataset for Symbolic Music Processing.* 2024.
> <https://zenodo.org/records/15571083>

Those files are unchanged. The `id` of a score is its score number on MuseScore.com. The `rating` and `ratings` fields
in the catalogue are the figures recorded in PDMX; a score without them was not rated.

## Scores from other editions

Nineteen scores (`own: true` in the catalogue, ids beginning with `ln-`) were made for LalaNote. The music of all of them
is in the public domain worldwide; the licence is that of the modern edition the file was made from, and each file
carries it in its MusicXML `<rights>` element.

| Score | Edition and licence |
|---|---|
| Beethoven, *Für Elise*, WoO 59 (complete, and the right hand alone) | Typeset by Stelios Samelis for the Mutopia Project (Mutopia-2015/08/18-931) after Breitkopf & Härtel, 1888. **Public Domain**. <https://www.mutopiaproject.org/cgibin/piece-info.cgi?id=931> |
| Pachelbel, *Canon in D* (3 violins and bass, and a reduction for piano) | Typeset by Michael Fischer v. Mollard for the Mutopia Project (Mutopia-2015/09/02-2047). **CC BY 4.0** — <https://creativecommons.org/licenses/by/4.0/>. Changes: converted from LilyPond to MusicXML; for the piano version, violin I and the bass set on two staves. <https://www.mutopiaproject.org/cgibin/piece-info.cgi?id=2047> |
| Mozart, 12 Variations on "Ah, vous dirai-je, Maman", K. 265 — theme and variations I–III | Transcribed by Eric Bréchemier from the autograph and the first edition (Vienna, 1785). **CC0 1.0**. Changes: the "D.C." of each section written out; the unfinished variations IV–XII left out. <https://github.com/eric-brechemier/mozart-kv265> |
| Twinkle, Twinkle, Little Star (words: Jane Taylor, 1806) · Happy Birthday to You · Ode to Joy (melody) · Joy to the World · Arirang | Public-domain melodies and original words, written out for LalaNote. **CC0 1.0**. No translated words: a translation has a copyright of its own. |
| Children's songs and folk songs, each a melody with its original words: Mary Had a Little Lamb (Lowell Mason, 1831; words Sarah Josepha Hale, 1830) · London Bridge Is Falling Down · Row, Row, Row Your Boat · Old MacDonald Had a Farm · Yankee Doodle · Hot Cross Buns · Jingle Bells (James Lord Pierpont, 1857) · Oh! Susanna (Stephen Foster, 1848; first verse and chorus) · Frère Jacques (French words) | Public-domain melodies and words, written out for LalaNote. **CC0 1.0**. They were written down from memory of the common versions and may differ from a particular printed one. |

## How the PDMX scores were chosen

The scores in PDMX were typed in by MuseScore.com users, who marked each one as public domain or CC0. That mark is
not always right, so only scores that pass all of the following are here:

1. PDMX found no licence conflict for the score, and the file is valid.
2. The composer is on a fixed list of composers who died in 1925 or earlier.
3. Nothing in the title or in the file names another arranger, transcriber, editor or translator. The only
   exceptions are arrangers who died long ago themselves, such as Liszt or Busoni.
4. Nothing in the file claims a copyright.
5. PDMX does not list it as a duplicate, and it is not marked as unfinished.
6. LalaNote opens it. A score that users rated (3.5 or higher; the catalogue gives the rating) may have up to one
   bar in ten that holds more beats than its time signature allows; a score nobody rated, one bar in fifty.

## What to expect

These are transcriptions made by volunteers. They can differ from a printed edition in notes, fingering, dynamics
or layout, and nobody has proofread them here. Sung words are as the uploader entered them; a score that names a
translator was left out, but an unnamed translation cannot be told apart from the original words. A bar may hold
more beats than its time signature allows.

## Licence

Each PDMX score carries the mark its uploader gave it, recorded in `catalog.json` as `CC0-1.0` or `Public Domain`.
The nineteen other scores are `CC0-1.0`, `Public Domain` or — the two Pachelbel files — `CC-BY-4.0`, which asks that the
typesetter be named when the file is passed on (see the table above).
`catalog.json` and this text are released under CC0 1.0. See [LICENSE.md](LICENSE.md).

## Reporting a problem

If a score here is yours and should not be, or is not free to share for any other reason, please
[open an issue](https://github.com/mylovejs2/LalaNoteOpenMusic/issues) naming the file. It will be taken out.
