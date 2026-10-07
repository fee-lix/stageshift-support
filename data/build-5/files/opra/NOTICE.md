# Headphone catalogue notice

The bundled headphone catalogue is adapted from the Open Headphone
Measurements and Equalizations Aggregation (OPRA) database at commit
`0b88ecd4e2bef7cf69fd5d50f1d06fb586c10865`.

- OPRA: https://github.com/opra-project/OPRA
- Catalogue license: Creative Commons Attribution-ShareAlike 4.0 International
- Exact adapted copy: the bundled/exported `catalogue.jsonl` (repository path
  `headphone-eq/normalized/catalogue.jsonl`)
- Changes: unsupported records were removed; one deterministic recommended
  parametric profile was selected per exact product; records were emitted in a
  versioned normalized field layout; and a separately declared constant safety
  trim may have been added to preserve at least 0.5 dB steady-state headroom.

OPRA includes data imported from AutoEq. The AutoEq software repository notice
is reproduced in `THIRD_PARTY_LICENSES.md`. Profile creator and source-detail
attribution are retained per record and displayed in the app. Each exported
record also identifies the immutable OPRA snapshot, license, accepted project
review decision, and this modification.

OPRA and profile-author names identify sources only. No endorsement or
affiliation is claimed. Manufacturer names identify compatible product models;
no manufacturer artwork is bundled.
