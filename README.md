# LalaNote Open Music

3,315 scores of classical music by 140 composers, as MusicXML (`.mxl`) files. They are the score library of the
[LalaNote](https://github.com/mylovejs2/LalaNote) score editor, and anyone may use them.

- `scores/<Composer>/<title>--<id>.mxl` — the scores
- `catalog.json` — one entry per score: title, composer, file, number of staves, parts, measures and pages, licence,
  and `lyrics: true` when the score has sung words

## Where the scores come from

Every file comes from **PDMX**, a dataset of public-domain MusicXML scores collected from MuseScore.com:

> Phillip Long, Zachary Novack, Taylor Berg-Kirkpatrick, Julian McAuley.
> *PDMX: A Large-Scale Public Domain MusicXML Dataset for Symbolic Music Processing.* 2024.
> <https://zenodo.org/records/15571083>

The files are unchanged. The `id` of a score is its score number on MuseScore.com. The `rating` and `ratings` fields
in the catalogue are the figures recorded in PDMX; a score without them was not rated.

## How they were chosen

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

Each score carries the mark its uploader gave it, recorded in `catalog.json` as `CC0-1.0` or `Public Domain`.
`catalog.json` and this text are released under CC0 1.0. See [LICENSE.md](LICENSE.md).

## Reporting a problem

If a score here is yours and should not be, or is not free to share for any other reason, please
[open an issue](https://github.com/mylovejs2/LalaNoteOpenMusic/issues) naming the file. It will be taken out.
