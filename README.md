# ErsatzRS Next runtime packages

This repository distributes pinned ErsatzTV Next runtime packages used by
ErsatzRS, with upstream source, compatibility patches, licence, provenance and
checksums. FFmpeg is distributed separately.

## Current runtime

- Version: `0.2.5-c5cb065-ersatzrs.1`
- [Release and downloads](https://github.com/bartdeijkers/ErsatzRS-next/releases/tag/next-0.2.5-c5cb065-ersatzrs.1)
- Upstream: `ErsatzTV/next`, revision `c5cb065f9f35dbbcb7c05845f0f92c70f576a480`.
- Packages: Linux x64, Linux ARM64, Linux ARMv7 and Windows x64.

The archives are the exact qualified packages, published without rebuilding.
Each archive has a provenance sidecar; `SHA256SUMS` covers the release assets.
ErsatzRS verifies archive and payload pins before executing Next.

Linux and native Windows software playback, available Windows CUDA and ARM
software emulation have scoped verification. Native ARM, macOS and unavailable
hardware remain unverified/deferred. No new macOS packages are supplied.
Application integration and acceptance are separate from package qualification.
ErsatzRS retains its selectable Native engine alongside Next.

## Source and temporary corrections

The release includes the exact upstream source archive, twelve patches, their
manifest, the source-preparation script and MIT licence. The corrections cover
bounded inputs, image repetition, dependency security, MPP readiness, selected
audio/caption clocks and finite ownership, plus the atomic indexed-playout
reader and package metadata. The manifest records each patch checksum and
retirement condition. Remove a correction when equivalent upstream behavior
passes its unchanged regression and compatibility checks; retain the tests.

The asset README records its pre-publication qualification state. These release
notes and the immutable checksums identify the published distribution.

## Licence

Next uses the upstream MIT licence, included as `LICENSE` in the release and
runtime archives.
