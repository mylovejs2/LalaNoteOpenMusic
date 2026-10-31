# LalaNote Open Music

3,610 scores of classical music and well-known tunes, as MusicXML (`.mxl`) files. They are the score library of the
[LalaNote](https://github.com/mylovejs2/LalaNote) score editor, and anyone may use them.

- `scores/<Composer>/<title>--<id>.mxl` — the scores
- `catalog.json` — one entry per score: title, composer, file, number of staves, parts, measures and pages, licence,
  and `lyrics: true` when the score has sung words. The scores that do not come from PDMX are marked
  `own: true` and name their edition in `credit`; the short practice versions among them are also marked `excerpt: true`

## Where the scores come from

All but 349 of the files come from **PDMX**, a dataset of public-domain MusicXML scores collected from MuseScore.com:

> Phillip Long, Zachary Novack, Taylor Berg-Kirkpatrick, Julian McAuley.
> *PDMX: A Large-Scale Public Domain MusicXML Dataset for Symbolic Music Processing.* 2024.
> <https://zenodo.org/records/15571083>

Those files are unchanged. The `id` of a score is its score number on MuseScore.com. The `rating` and `ratings` fields
in the catalogue are the figures recorded in PDMX; a score without them was not rated.

## Scores from other editions

349 scores (`own: true` in the catalogue, ids beginning with `ln-`) were made for LalaNote. The music of all of them
is in the public domain worldwide; the licence is that of the modern edition the file was made from, and each file
carries it in its MusicXML `<rights>` element.

323 of them, titled "— practice excerpt" and marked `excerpt: true`, are the built-in practice pieces of the Lala Keys
piano app: a short piece whole (the teaching pieces of Beyer and Czerny, up to 32 bars), a longer one its opening
section and close (12–24 bars), transcribed from the edition named below and checked bar by bar against it. Ties are
shortened to the bar line, ornaments and grace notes left out, and a piece that moves in triplets throughout is written
in 6/8, 9/8 or 12/8, which sounds the same. They carry no fingering. A hand's staff changes clef where the edition's
does (a change inside a bar is made at a bar line); in the pieces whose clefs were not taken from the edition, where
that keeps the notes on the staff. LalaNote lists them after the whole scores.

| Score | Edition and licence |
|---|---|
| Beethoven, *Für Elise*, WoO 59 (complete, and the right hand alone) | Typeset by Stelios Samelis for the Mutopia Project (Mutopia-2015/08/18-931) after Breitkopf & Härtel, 1888. **Public Domain**. <https://www.mutopiaproject.org/cgibin/piece-info.cgi?id=931> |
| Pachelbel, *Canon in D* (3 violins and bass, and a reduction for piano) | Typeset by Michael Fischer v. Mollard for the Mutopia Project (Mutopia-2015/09/02-2047). **CC BY 4.0** — <https://creativecommons.org/licenses/by/4.0/>. Changes: converted from LilyPond to MusicXML; for the piano version, violin I and the bass set on two staves. <https://www.mutopiaproject.org/cgibin/piece-info.cgi?id=2047> |
| Mozart, 12 Variations on "Ah, vous dirai-je, Maman", K. 265 — theme and variations I–III | Transcribed by Eric Bréchemier from the autograph and the first edition (Vienna, 1785). **CC0 1.0**. Changes: the "D.C." of each section written out; the unfinished variations IV–XII left out. <https://github.com/eric-brechemier/mozart-kv265> |
| Twinkle, Twinkle, Little Star (words: Jane Taylor, 1806) · Happy Birthday to You · Ode to Joy (melody) · Joy to the World · Arirang | Public-domain melodies and original words, written out for LalaNote. **CC0 1.0**. No translated words: a translation has a copyright of its own. |
| Children's songs and folk songs, each a melody with its original words: Mary Had a Little Lamb (Lowell Mason, 1831; words Sarah Josepha Hale, 1830) · London Bridge Is Falling Down · Row, Row, Row Your Boat · Old MacDonald Had a Farm · Yankee Doodle · Hot Cross Buns · Jingle Bells (James Lord Pierpont, 1857) · Oh! Susanna (Stephen Foster, 1848; first verse and chorus) · Frère Jacques (French words) · Au clair de la lune (French words) · Alle meine Entchen · Hänschen klein (words Franz Wiedemann, 1860) · O Tannenbaum (words Ernst Anschütz, 1824) · Stille Nacht, heilige Nacht (Franz Xaver Gruber, 1818; words Joseph Mohr, 1816) (German words, first verses) · Sakura Sakura (Japanese words) · Grandfather's Clock (words and music by Henry Clay Work, 1876; first verse and chorus, after the first edition) | Public-domain melodies and words, written out for LalaNote. **CC0 1.0**. They were written down from memory of the common versions and may differ from a particular printed one. |
| Czerny, *30 Études de mécanisme*, Op. 849 — Nos. 1–30, practice excerpts | Transcribed from the edition typeset by Neru Hayashi (IMSLP #612302), dedicated to the public domain. **Public Domain**. <https://imslp.org/wiki/Special:ImagefromIndex/612302> |
| Clementi, 6 Sonatinas, Op. 36 — No. 1 (three movements) and the first movements of Nos. 2–6, practice excerpts | Transcribed from the edition typeset by Nicholas Bosse (IMSLP #725302). **CC BY 4.0** — <https://creativecommons.org/licenses/by/4.0/>. Changes: transcribed to MusicXML and shortened for practice. <https://imslp.org/wiki/Special:ImagefromIndex/725302> |
| Burgmüller, *25 Études faciles et progressives*, Op. 100 — Nos. 1–8 and 10, practice excerpts | Transcribed from the Mutopia Project editions typeset by Bas Wassink after the Collection Litolff (Mutopia ids 202, 203, 214–219, 221). **Public Domain**. <https://www.mutopiaproject.org/> |
| Burgmüller, Op. 100 — Nos. 11–15 and 19–25, practice excerpts | Transcribed from the edition typeset by Ruiming Zhang (IMSLP #935040). **CC BY 4.0** — <https://creativecommons.org/licenses/by/4.0/>. Changes: transcribed to MusicXML and shortened for practice. <https://imslp.org/wiki/Special:ImagefromIndex/935040> |
| Dussek, Sonatina Op. 20 No. 1, first movement · Beethoven (attributed), Sonatina in F major, Anh. 5 No. 2, first movement · C. P. E. Bach, March in D major, BWV Anh. 122 · Tchaikovsky, *Children's Album*, Op. 39 Nos. 8, 15 and 21 — practice excerpts | Transcribed from public-domain editions on IMSLP: G. Schirmer, 1894 (#09896); Breitkopf & Härtel, *Beethovens Werke*, Serie 16 No. 161 (#51817); *Neue Bach-Ausgabe* V/4, 1957 (#867479); G. Schirmer, 1904 (#07996). The last three were also checked against PDMX scores 1635126, 5534866 and 5329984 (CC0). **Public Domain**. |
| Czerny, *Erster Wiener Lehrmeister*, Op. 599 (100 studies) — Nos. 1–100, practice versions | Transcribed from the edition typeset by Yufan, 2023 (IMSLP #856415). **CC0 1.0**. <https://imslp.org/wiki/Special:ImagefromIndex/856415> |
| Beyer, *Vorschule im Klavierspiel*, Op. 101 — Nos. 1–106, practice versions (the pupil's part where Beyer prints a teacher's part) | Transcribed from Edition Peters, ed. Adolf Ruthardt [1895] (IMSLP #12916). **Public Domain**. <https://imslp.org/wiki/Special:ImagefromIndex/12916> |
| Schumann, Träumerei · Brahms, Wiegenlied (arr. Robert Keller) · Bach, Air BWV 1068 (arr. Siloti) · Grieg, Morgenstimmung (the composer's piano version) · Tchaikovsky, *Swan Lake* Act II Scène (piano reduction by Kashkin) · Mozart, Rondo alla Turca · Chopin, Preludes Op. 28 Nos. 15 and 20 · Schubert, Ständchen (Liszt S. 560/7) · Debussy, Première Arabesque · Mendelssohn, Frühlingslied Op. 62 No. 6 · Dvořák, Humoresque Op. 101 No. 7 (ed. Godowsky) · Bądarzewska, La prière d'une vierge · Beethoven (attributed), Sonatina in G, Anh. 5 No. 1 · Kuhlau, Sonatina Op. 55 No. 1 — practice excerpts | Transcribed from public-domain editions, each named in its file's credit: IMSLP #289791, #10047, #09510, #88818, #1054921, #821296, #100461, #254504, #994954, #11082, #32596, #994931, #882995, and the Mutopia Project editions 471 and 472. **Public Domain**. |
| Chopin, Waltz in A minor, B. 150 — practice excerpt | Transcribed from the edition typeset by Rain Zhang, 2025 (IMSLP #968535). **CC0 1.0**. |
| Schumann, *Kinderszenen* No. 1 "Von fremden Ländern und Menschen" · Beethoven, Minuet in G (Sonata Op. 49 No. 2, II) · Chopin, Prelude Op. 28 No. 4 and Études Op. 10 Nos. 5 and 12 · Grieg, In the Hall of the Mountain King (the composer's piano version) · Mozart, Fantasia in D minor, K. 397 · Schubert, Impromptus Op. 90 Nos. 2 and 4, and Die Forelle (the voice and the bass of the song) · Gounod, Ave Maria (the violin's melody and the bass of the piano) — practice excerpts | Transcribed from the Mutopia Project editions 354, 777, 468, 926, 743, 1888, 2034, 1551, 1552, 502 and 2167, each named in its file's credit. **Public Domain**. <https://www.mutopiaproject.org/> |
| Chopin, Polonaise Op. 53 · Beethoven, Sonata Op. 31 No. 2, III · Liszt, La Campanella S. 141 No. 3 · Tchaikovsky, Danse de la Fée-Dragée and Valse des fleurs (the composer's piano arrangement of the Nutcracker suite) · Saint-Saëns, Le Cygne (piano transcription by Alexander Siloti) · Verdi, "La donna è mobile" (the voice and the bass) · Johann Strauss II, An der schönen blauen Donau (the composer's piano version) · Boccherini, Minuet (piano arrangement by Albert E. Wier) · Elgar, Salut d'Amour (the composer's piano version) — practice excerpts | Transcribed from public-domain editions on IMSLP, each named in its file's credit: #42524, #419638, #29890, #57454, #10939, #88973, #311227, #796689, #167967. **Public Domain**. |
| Beethoven, Minuet in G, WoO 10 No. 2 · Mozart, *Eine kleine Nachtmusik*, K. 525, I (arr. Otto Singer) · Offenbach, Barcarolle from *Les contes d'Hoffmann* (arr. Auguste Bazille) · Wagner, Bridal Chorus from *Lohengrin* (arr. Gustav Lazarus) · The Londonderry Air (Petrie Collection, 1855) · Cottrau, Santa Lucia · Elgar, Land of Hope and Glory (the song, 1902) · Holst, *The Planets*: Jupiter, the big tune (the first violins and the double basses) · Schubert, Ave Maria, D. 839 — practice excerpts, the melody and the bass | Transcribed from public-domain editions on IMSLP, each named in its file's credit: #993206, #61339, #02610, #286240, #395124, #318686, #556094, #15436, #62384. **Public Domain**. |
| Burgmüller, 18 Études Op. 109 — Nos. 1, 2, 8, 13 and 15, practice excerpts | Collection Litolff No. 2364, ed. Clemens Schultze [1905] (IMSLP #283546). **Public Domain**. |
| Mozart, Piano Sonata in C, K. 545, first movement — practice excerpt | Transcribed from Craig Stuart Sapp's re-engraving of the Breitkopf & Härtel Mozart edition, 1878 (IMSLP #1020082). **CC BY 4.0** — <https://creativecommons.org/licenses/by/4.0/>. Changes: transcribed to MusicXML and shortened for practice. |

## How the PDMX scores were chosen

The scores in PDMX were typed in by MuseScore.com users, who marked each one as public domain or CC0. That mark is
not always right, so only scores that pass all of the following are here:

1. PDMX found no licence conflict for the score, and the file is valid.
2. The composer is on a fixed list of composers who died in 1925 or earlier.
3. Nothing in the title or in the file names another arranger, transcriber, editor or translator. The only
   exceptions are arrangers who died long ago themselves, such as Liszt or Busoni.
4. Nothing in the file claims a copyright.
5. PDMX does not list it as a duplicate, it is not marked as unfinished, and no other score here has exactly the
   same notes (of such re-uploads the one with the most ratings is kept).
6. LalaNote opens it. A score that users rated (3.5 or higher; the catalogue gives the rating) may have up to one
   bar in ten that holds more beats than its time signature allows; a score nobody rated, one bar in fifty.

## What to expect

These are transcriptions made by volunteers. They can differ from a printed edition in notes, fingering, dynamics
or layout, and nobody has proofread them here. Sung words are as the uploader entered them; a score that names a
translator was left out, but an unnamed translation cannot be told apart from the original words. A bar may hold
more beats than its time signature allows.

## Licence

Each PDMX score carries the mark its uploader gave it, recorded in `catalog.json` as `CC0-1.0` or `Public Domain`.
The 349 other scores are `CC0-1.0`, `Public Domain` or — the two Pachelbel files, the eight Clementi movements, twelve of
the Burgmüller études and the K. 545 movement — `CC-BY-4.0`, which asks that the typesetter be named when the file is
passed on (see the table above).
`catalog.json` and this text are released under CC0 1.0. See [LICENSE.md](LICENSE.md).

## Reporting a problem

If a score here is yours and should not be, or is not free to share for any other reason, please
[open an issue](https://github.com/mylovejs2/LalaNoteOpenMusic/issues) naming the file. It will be taken out.
