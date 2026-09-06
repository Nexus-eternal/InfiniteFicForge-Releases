# Infinite Fic Forge

**Infinite Fic Forge (IFF)** is a Windows desktop app for building and maintaining long-running AI-assisted fiction projects: chapter generation, story planning, a living Canon Wiki, progression tracking, illustrations, backups and portable project export.

This repository is the **public binary distribution home** for IFF. Source development currently happens separately.

## Download

Open **Releases** and download the newest stable version.

For most users:

- `InfiniteFicForge-<version>-Setup.exe` — normal Windows installer.
- `InfiniteFicForge-<version>-portable-windows-x64.zip` — portable build without installation.

Each release also includes SHA-256 checksums and updater metadata.

## What IFF includes

- Long-form chapter generation with planning, critic passes and resumable checkpoints.
- Project Canon Wiki, Reference Canon / Setting Packs and provenance.
- Saga / Arc story planning and progression support.
- OpenAI, Claude, Venice, OpenAI-compatible and local AI endpoints.
- Illustration generation with visual continuity and semantic QA.
- Crash recovery, Backup / Restore and `.iff-project` portability.
- Russian and English desktop UI, built-in Help Center and demo project.

## API providers and local data

IFF does **not** include an AI subscription. You connect your own supported provider or local endpoint, and provider usage may incur charges according to that provider's pricing.

Books and project data are stored locally in the Library directory you choose. API credentials are stored through the operating-system credential store where supported.

## Current 1.0 limitation

The desktop UI supports Russian and English, but the 1.0 generation pipeline is still Russian-first. English projects can currently receive Russian prose or Canon updates during later AI-generated chapters. Full per-project content-language enforcement is planned after 1.0.

## Windows warning

Early public builds are not code-signed yet, so Windows SmartScreen may display an unknown-publisher warning. Code signing is planned as a separate hardening step.

## Update feeds

- `latest.json` — newest stable release.
- `beta.json` — newest build including prereleases.

IFF verifies downloaded update metadata against published byte sizes and SHA-256 hashes before installation.
