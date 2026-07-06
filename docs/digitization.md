# Digitization Workflow

Playback transfer follows physical stabilization and cleaning. This document outlines the transfer chain and digital preservation targets for the St. Luke's / KTOK transcription set.

## Playback

- **Turntable:** 16"-capable transcription turntable (documented in process photography alongside legacy KUT/broadcast equipment).
- **Speed:** 33⅓ RPM per label.
- **Direction:** **Inside start** — labels are marked "Start Inside"; cue the stylus at the innermost groove.
- **Stylus:** Appropriately sized truncated stylus selected per disc groove profile (transcription discs frequently require 2.5–4.0 mil; verify by test tracking rather than assuming microgroove or standard 78 sizes).
- **Equalization:** Flat transfer preferred at capture; broadcast-era EQ curve applied or documented in post.

## Capture Targets

| Parameter | Preservation master | Access copy |
|---|---|---|
| Format | BWF (.wav) | MP3/AAC |
| Bit depth / rate | 24-bit / 96 kHz | 320 kbps / 44.1 kHz |
| Channels | Mono capture retained as recorded | Mono |
| Metadata | Embedded BWF bext + sidecar (PBCore/PREMIS) | ID3 |

## Documentation Standards

- One condition photograph set per disc: full face, label detail, raking-light groove detail — before, during, and after treatment (51 images total across the set).
- Filenames: `YYYY-MM-DD_disc#_description.JPG` keyed to recording date on the label.
- Captions and descriptive metadata maintained in `metadata/image-captions.csv`.

## Quality Control

- A/B review of transfer against disc surface condition notes.
- Declicking and restoration performed only on access derivatives; preservation master remains flat/unprocessed.
- Checksums (SHA-256) generated at capture and verified on ingest.
