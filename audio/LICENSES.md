# Audio licenses

All audio is recorded/produced material released under **CC0 1.0 Universal (public domain dedication)**, https://creativecommons.org/publicdomain/zero/1.0/ . No attribution is required; credit is given anyway. Nothing is synthesised in code (Playgama rule 3.3.2).

Processing done by us (ffmpeg): mono down-mix, loudness normalisation (EBU R128 `loudnorm`, SFX -18 LUFS, music -20 LUFS), encode to Ogg Vorbis (q3) and MP3 fallback. Files are chosen at runtime with `canPlayType` (ogg, else mp3). The music is the unedited 64 s loop; the author renders his tracks so that they loop.

| File | Use | Original | Source URL | License | Provenance / evidence |
|---|---|---|---|---|---|
| music_loop.ogg / .mp3 | Background music loop (64 s) | "Free as a Bird" by Harm-Jan "3xBlast" Wiechers, from "3xBlast - Free Music Pack (15 songs)" | https://opengameart.org/node/97953 | CC0 1.0 | Primary source opened in a browser on 2026-11-22: page "3xBlast - Free Music Pack (15 songs)", License(s): CC0 (public-domain badge), author text "All these songs are licensed under CC0 1.0 Universal ... you can use 'em for whatever, whenever". The file itself was obtained from the GitHub mirror https://github.com/Andrew231716/visionai-music (commit c68a019, audio/travel/travel_006.mp3, sha256 7923d0d61738d180fdc28770861dcd7d001b8df08a59f5b75bb43e9b33ebf434; mirror records license CC0-1.0 and the same source page, see licenses/music-mirror_free-as-a-bird_manifest-entry.json).  |
| sfx_slither.ogg / .mp3 | Snake slithers out (variant A) | scroll_002 - Kenney "Interface Sounds" | https://kenney.nl/assets/interface-sounds | CC0 1.0 | GitHub port https://github.com/Calinou/kenney-interface-sounds (clone at commit 4596a49); pack LICENSE.txt: "License: (Creative Commons Zero, CC0)". Source file scroll_002.wav sha256 a6cf83057f2e66a6744cbfcef5dcb6705a875e2d86f908f4f6ef9cac5113999a; shipped sfx_slither.ogg sha256 cb6df570883325a36e5ffe665dc6c4da316b47835f620b014a176b33111c6e6d. Chosen because the soft scraping swish reads as a body gliding over stone, softer than the cloth whoosh used before. |
| sfx_slither2.ogg / .mp3 | Snake slithers out (variant B) | scroll_003 - Kenney "Interface Sounds" | same | CC0 1.0 | Same pack. Source file scroll_003.wav sha256 0b5781b18dfa8eed60f3bca9a964785fdbeb823a046c81099bca8cbf9a09804d; shipped sfx_slither2.ogg sha256 08a8b869c5449fa85f8f9909215de36aca6ded861a765aa1fd6f3d138989b48d. |
| sfx_gust.ogg / .mp3 | Hint reveal | cloth_1 - Kenney "RPG Audio" | same | CC0 1.0 | same |
| sfx_bump.ogg / .mp3 | Blocked snake bumps | impact_soft_heavy_001 - Kenney "Impact Sounds" | https://kenney.nl/assets/impact-sounds | CC0 1.0 | GitHub port https://github.com/Boyquotes/kenney-impact-sounds-for-godot, repo LICENSE = CC0 1.0 legal text |
| sfx_gameover.ogg / .mp3 | Level failed | impact_bell_heavy_002 - Kenney "Impact Sounds" | same | CC0 1.0 | same |
| sfx_clear.ogg / .mp3 | Level cleared (1-2 stars) | confirmation_002 - Kenney "Interface Sounds" | https://kenney.nl/assets/interface-sounds | CC0 1.0 | GitHub port https://github.com/Calinou/kenney-interface-sounds; pack LICENSE.txt: "License: (Creative Commons Zero, CC0)" |
| sfx_combo.ogg / .mp3 | Level cleared with 3 stars | confirmation_004 - Kenney "Interface Sounds" | same | CC0 1.0 | same |
| sfx_click.ogg / .mp3 | Button click | click_001 - Kenney "Interface Sounds" | same | CC0 1.0 | same |

## Copies of the license texts kept with the build (`licenses/`)

- `kenney-interface-sounds_pack-LICENSE.txt`, `kenney-interface-sounds_LICENSE.txt` - Kenney Interface Sounds pack license (CC0) and port repo license
- `kenney-impact-sounds_repo-LICENSE-CC0.txt` - CC0 1.0 legal text from the Impact Sounds port repo
- `kenney-rpg-audio_repo-LICENSE-CC0.txt` - CC0 1.0 legal text from the RPG Audio port repo (still used for the hint sound, sfx_gust, cloth_1)
- `music-mirror_free-as-a-bird_manifest-entry.json`, `music-mirror_SOURCE_VERIFICATION.md` - the mirror's recorded verification

## Open points

- The music track file comes through a third-party mirror (the OpenGameArt page itself was opened and shows CC0 for the whole pack, but the per-file link is the mirror). The track's character was not auditioned by ear in this sandbox: listen to it once before publishing.
- The RPG Audio port repo only ships the generic CC0 legal text; the pack is CC0 on https://kenney.nl/assets/rpg-audio.

## sfx_hiss.ogg / sfx_hiss.mp3 (slither sound, added 2026-11-22)
- Source: "hiss2.wav" by Reitanna, Freesound sound 343927 - https://freesound.org/people/Reitanna/sounds/343927/
- License: Creative Commons 0 (CC0 1.0), checked on the original page on 2026-11-22 (license link: http://creativecommons.org/publicdomain/zero/1.0/). Full text: licenses/CC0-1.0-legalcode.txt
- Downloaded by the owner from Freesound (logged-in download); original 0.64 s, 44.1 kHz mono 16-bit, 56,364 bytes.
- Original sha256: dc48c5a5c642a5efc50c0ea4288de69bb8eda2d56812c76c893eaf13b84fd824
- Processing (tools/process_hiss.py): trimmed to 0.5 s, loudness-normalised (-18 LUFS), 15 ms fade-in, 120 ms fade-out. Recorded audio, not synthesised.
- sfx_hiss.ogg sha256: 6659d4584c8c655f5b9b4d041a9aafaaeed05083a00ecadd0c481a6bdb171081
- sfx_hiss.mp3 sha256: 77086a667bd1401437874f3f627ec93dff490173592f1bc9712c25f80599713e
