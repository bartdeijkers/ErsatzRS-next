# ErsatzRS Next runtime packages

This repository distributes pinned ErsatzTV Next runtime packages used by
ErsatzRS. It contains dependency packages, their upstream source archive,
compatibility patches, licence, provenance and checksums.

## Current runtime

- Version: `0.1.0-0362692-ersatzrs.1`
- Release tag: `next-0362692-ersatzrs.1`
- Upstream: `ErsatzTV/next`, revision `03626929089a438245cfc77cbedda6e92d98dc9f`
- Platforms: Linux x64, ARM64 and ARMv7; Windows x64; macOS x64 and ARM64.

These are the existing verified packages, copied without rebuilding or changing
any package bytes. Each archive has its own provenance sidecar; `SHA256SUMS`
records the published asset checksums. The ErsatzRS runtime verifies its exact
archive and payload pins before executing Next.

Linux and Windows have application playback evidence. ARM and macOS packages
have build/package evidence; their application acceptance remains explicitly
unverified. No new platform or hardware validation is claimed by this mirror.

## Temporary compatibility patches

The release contains the bounded live RTSP buffering and programme-image repeat
patches together with the reviewed upstream source. They must be removed once
upstream provides equivalent corrections and the existing regression and
compatibility checks pass. The tests remain.

## Licence

Next is distributed under its upstream MIT licence, included as `LICENSE` in the
release and runtime archives. FFmpeg is distributed separately.
