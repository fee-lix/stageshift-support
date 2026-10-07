# Preset Licenses

This directory contains the Slice 6.2/V2 runtime preset bundle candidate. The
nine rendered assets below are available to development builds and the
explicit Android/iOS closed Beta. `direct` requires no room asset. Retained
legacy candidate sources stay blocked until a future preset review accepts
them for a product room set.

## Current bundled candidate assets

| Preset | Runtime asset | Source | License |
| --- | --- | --- | --- |
| `practice_room` | `ir/practice_room_openair_peak_minus6.wav` | OpenAIR Maes Howe `mh3_000_ortf_48k.wav` | CC BY 4.0 |
| `studio_room` | `ir/studio_room_openair_peak_minus6.wav` | OpenAIR Genesis 6 Studio `kick_ir.wav` | CC BY 4.0 |
| `chamber_room` | `ir/chamber_room_openair_peak_minus6.wav` | OpenAIR Dixon Studio Theatre `r1_rir_bformat.wav` | CC BY 4.0 |
| `concert_hall` | `ir/concert_hall_openair_peak_minus6.wav` | OpenAIR Usina del Arte Symphony Hall `usina_main_s1_p5.wav` | CC BY 4.0 |
| `church` | `ir/church_openair_peak_minus6.wav` | OpenAIR York Minster `minster1_000_ortf_48k.wav` | CC BY 4.0 |
| `opera` | `ir/opera_openair_peak_minus6.wav` | OpenAIR Theatre@41 `theatre41_CenterAVG_32_48.wav` | CC BY 4.0 |
| `grand_concert_hall` | `ir/grand_concert_hall_openair_peak_minus6.wav` | OpenAIR Jack Lyons Concert Hall `rir_jack_lyons_lp2_96k.wav` | CC BY 4.0 |
| `ceremonial_hall` | `ir/ceremonial_hall_openair_peak_minus6.wav` | OpenAIR Elveden Hall `1a_marble_hall.wav` | CC BY 4.0 |
| `cathedral` | `ir/cathedral_openair_peak_minus6.wav` | OpenAIR York Minster `minster1_000_ortf_48k.wav` | CC BY 4.0 |

Each candidate has a per-preset `license.txt`, `recipe.json`, and manifest
hashes for the source and rendered file. The release preset gate remains blocked
pending listening review, CPU/runtime review, and final preset QA.

Packages containing these assets must include this overview and each room's
`license.txt` and `recipe.json` in `PresetLegal`, available on the offline
Licenses page. The license files identify creators, source pages, and the
CC BY 4.0 license URI. The recipes describe modifications including peak
normalization, channel decoding, and resampling where applied. Closed-beta
availability does not change `blocked_pending_release_review` or include the
unrendered legacy candidates.

## Blocked candidate sources

`classroom` and `small_hall` record candidate source URLs, licenses,
attribution, and hashes, but expose no playable runtime IR asset in
`presets/presets.json`. Their block reasons are in `presets/presets.json` and
per-preset `license.txt` files.

## License policy for future assets

Each bundled preset must include a clear license trail before it can ship:

- source name and author/owner;
- source URL or internal measurement record;
- license type and license text or link;
- attribution text;
- source-file hash;
- rendered-file hash;
- processing recipe;
- confirmation that redistribution in a free open-source mobile app is permitted.

## Blocked assets

Do not add IRs or samples with unclear redistribution terms, non-commercial-only terms unless explicitly approved for the project use case, GPL/AGPL-like binary constraints, missing attribution requirements, or unclear recording-location rights.
