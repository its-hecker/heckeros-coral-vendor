# HeckerOS coral vendor

Based on the existing PixelOS coral vendor snapshot in UPSTREAM_SOURCE.json. Hardware blobs, extraction metadata, install ownership fixes and original licenses are retained. All 11 radio payloads are fetched from the existing public Git LFS read endpoint in .lfsconfig and verified against Android.mk by the LFS workflow. No external LFS upload credentials are required for read-only builds.

Use the [HeckerOS coral local manifest](https://github.com/its-hecker/HeckerOs-localmanifest) for pinned source/build setup. ROM customizations, FaceID and Motion Sense integration, GCam, Settings and branding belong to [HeckerOS](https://github.com/its-hecker/HeckerOS). Full ROM build and coral validation are pending.

## SIM Manager update — 9 November 2026

The XDA improvements branch updates only EuiccGoogle to Google-signed
`D.2.1.989982212-google` (306110), extracted from the shared modified Flame ROM.
Its original v3 signature, SHA-256, product packaging and native-library alignment
are verified. The pinned Suite supplies its five additional privileged permissions.
See `provenance/EuiccGoogle.json` for exact provenance and the permission audit.
Full ROM and physical eSIM setup validation remain pending.
