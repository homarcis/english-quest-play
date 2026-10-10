# Asset licenses

Every visual or audio asset used in English Quest must be listed here (NFR-08). Assets are either CC0 or original art owned by the project author (see "Original art" below).

## Original art (S8, default look)

Created by the project author, Homar Cisneros, with ChatGPT image generation, based on the game's earlier designs (2026-10-09). Owned by the author and used with the author's permission; not CC0. Files in `public/assets/art/`:

| File | Made from | Processing |
|---|---|---|
| `hub.webp` | Plaza (1447×1087) | Scaled to 960×721 (Lanczos), cropped to 960×720, WebP q90 |
| `cafe.webp` | Café interior (1672×941) | Scaled to 960×540 (Lanczos), WebP q90 |
| `cafe-counter.webp` | Same café picture | Counter front cut out (x 553, y 176, 394×67) and drawn over the barista |
| `player.png`, `clara.png`, `sam.png` | Character sprites (1254×1254, transparent) | Transparent border trimmed, scaled to 192 px high (shown at 76–100 px) |
| `laptop.png` | Laptop sprite (1254×1254, transparent) | Trimmed, scaled to 96 px wide (shown at 52 px) |

The separate Café and Academy building images were not needed (the plaza picture already contains both) and are not shipped.

The classic look below (`VITE_LOOK=classic`) still uses the CC0 sprites and code-drawn shapes.

## CC0 assets

| Asset / pack | Files in the project | Author | Source URL | License | Date added |
|---|---|---|---|---|---|
| Roguelike Indoors | `public/assets/kenney/roguelike-indoors.png` (renamed from `roguelikeIndoor_transparent.png`), `LICENSE-roguelike-indoors.txt` | Kenney (kenney.nl) | https://kenney.nl/assets/roguelike-indoors | CC0 1.0 | 2026-10-08 |
| Cozy Asset Pack 1.0 (characters) | `public/assets/ishtar/player.png`, `sam.png`, `clara.png` (cropped from `top-down-pack-2.png`), `LICENSE-cozy-asset-pack.txt` | Ishtar Pixels | https://opengameart.org/content/cozy-asset-pack-10 | CC0 1.0 | 2026-10-08 |

## Sound (S7)

All sound files live in `public/assets/sound/` and are CC0 1.0. They were re-encoded to MP3 (so every browser, Safari included, can play them); ambience was converted to mono and given short fades so the loop point is smooth.

| Asset | Files in the project | Author | Source URL | License | Date added |
|---|---|---|---|---|---|
| Interface Sounds | `sfx/tap.mp3` (click_001), `place.mp3` (pluck_001), `success.mp3` (confirmation_002), `retry.mp3` (error_006), `hint.mp3` (question_001), `LICENSE-kenney-interface-sounds.txt` | Kenney (kenney.nl) | https://kenney.nl/assets/interface-sounds | CC0 1.0 | 2026-10-09 |
| RPG Audio | `sfx/door.mp3` (doorOpen_1), `step1.mp3`, `step2.mp3` (footstep00, footstep01), `page.mp3` (bookFlip1), `LICENSE-kenney-rpg-audio.txt` | Kenney (kenney.nl) | https://kenney.nl/assets/rpg-audio | CC0 1.0 | 2026-10-09 |
| Music Jingles | `sfx/complete.mp3` (jingles_PIZZI03), `LICENSE-kenney-music-jingles.txt` | Kenney (kenney.nl) | https://kenney.nl/assets/music-jingles | CC0 1.0 | 2026-10-09 |
| Chill lofi inspired [loop edit] | `loops/hub-music.mp3` | qubodup | https://opengameart.org/content/chill-lofi-inspired-loop-edit | CC0 1.0 | 2026-10-09 |
| Park ambiences (birds) | `loops/hub-birds.mp3` (40 s from 1:00 of park_ambience_birds.wav, mono, fades) | Thimras | https://opengameart.org/content/park-ambiences | CC0 1.0 | 2026-10-09 |
| Coffee House Bump | `loops/cafe-music.mp3` (little_cafe_jazz.mp3) | oatcog | https://opengameart.org/content/coffee-house-bump | CC0 1.0 | 2026-10-09 |
| Crowded Pub | `loops/cafe-murmur.mp3` (crowded_pub_2025_2.mp3, mono, fades) | bobjt | https://opengameart.org/content/crowded-pub | CC0 1.0 | 2026-10-09 |
| Calm Piano 1 (Vaporware) | `loops/academy-music.mp3` (003_Vaporware_2.mp3) | cynicmusic | https://opengameart.org/content/calm-piano-1-vaporware | CC0 1.0 | 2026-10-09 |

Each OpenGameArt page lists CC0 as its only license (checked on 2026-10-09). The menu credits every author.

There is no text-to-speech in the app: the S6 listening activities that used the browser's voice were removed at the player's request.

Both packs ship a license file stating CC0; the original files are kept next to the images. Credit is not required, but the app's menu credits both authors.

The floor, walls, windows and door are drawn in code. The World Hub plaza (buildings, fountain, trees, benches, lamps) is drawn in code from `src/world/hubTheme.ts`; the Hub avatar reuses `public/assets/ishtar/player.png`.

## Modifications

- **clara.png** is a derivative of the light-haired character (sheet position x=80, y=176, 32×32): long hair was added on both sides of the face (rows 9–22), using the character's own hair palette. CC0 allows modification.
- **player.png** (x=48, y=176) and **sam.png** (x=112, y=176) are unmodified crops.

## Sprite frames used (Kenney Indoors)

Sheet of 16 × 16 px tiles with 1 px spacing, 27 columns. Frame = row × 27 + column.

| Use | Frames |
|---|---|
| Window table + chairs | 7, 56, 57 |
| Counter | 413, 414, 330, 415 |
| Desk, monitor, desk chair | 0, 1, 2, 129, 54 |
| Plant, bookshelf, picture | 16, 479, 340 |

## Removed

- Kenney Roguelike Characters (2026-10-08): replaced by the Ishtar Pixels characters.
