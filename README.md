# strudel-samples

Personal sample library for Strudel patches.

Load it in a patch or in Strudel's prebake:

```js
samples('github:<your-username>/strudel-samples')
```

## Sounds

- `vox` (23): breathy held vocal notes, retuned to C# minor, mono, 44.1 kHz.
  Grouped by pitch: `vox:0` B3 · `vox:1`-`vox:14` C#4 (`vox:9` is an 8 s hold) ·
  `vox:15`-`vox:16` D#4 · `vox:17`-`vox:18` E4 · `vox:19`-`vox:22` F#4
- `voxphrase` (4): longer phrases (14-35 s) for granular / ghost treatments
- `voxhit` (18): short, steady sung hits (0.15-0.8 s), retuned from D# minor to
  C# minor, sorted low to high: `voxhit:0` F#3 · `:1` B3 · `:2`-`:5` C#4 ·
  `:6`-`:7` D#4 · `:8`-`:9` G#4 · `:10` A4 · `:11`-`:12` B4 · `:13`-`:14` C#5 ·
  `:15` D#5 · `:16` E5 · `:17` F#5
- `voxswell` (8): longer sung swells (1.6-3.5 s), most with a glide in them:
  `voxswell:0`-`:1` A3 · `:2` B3 · `:3`-`:5` C#4/D#4 · `:6`-`:7` C#5

Vocals generated with Google Flow Music (Lyria 3.5), retuned to C# minor
(the pads up a semitone from C minor, the hits down two from D# minor) and trimmed.

## Adding sounds

Put audio in a folder (the folder name becomes the sound name), then regenerate
the index from the repo root:

```sh
npx --yes @strudel/sampler --json > strudel.json
```
