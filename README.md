# InfiniteFicForge-Releases

Public binary distribution mirror for **Infinite Fic Forge**.

This repository intentionally does **not** contain the private application source code. It is used only for public desktop release artifacts and updater feed metadata.

## Distribution layout

- GitHub Releases: versioned Windows installer and ZIP artifacts.
- `latest.json`: Stable channel feed.
- `beta.json`: Beta channel feed (prereleases plus the newest stable final).
- SHA-256 hashes are embedded in feed metadata and verified by the IFF updater before installation.

Source development remains in the private `Nexus-eternal/InfiniteFicForge` repository.
