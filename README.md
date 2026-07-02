# Maestro — Releases

![Latest release](https://img.shields.io/github/v/release/uitlaber/maestro-releases?label=latest&sort=semver)

Signed, notarized macOS builds of **Maestro** and the [Sparkle](https://sparkle-project.org) appcast that powers in-app auto-update.

## Download

**[⬇︎ Download the latest Maestro.dmg](https://github.com/uitlaber/maestro-releases/releases/latest/download/Maestro.dmg)**

Or pick any build from the [Releases page](https://github.com/uitlaber/maestro-releases/releases).

## Install

1. Open the downloaded `Maestro.dmg`.
2. Drag **Maestro.app** into **Applications**.
3. Launch it. The app is Developer ID–signed and notarized by Apple, so Gatekeeper opens it without warnings.

Requires **macOS 15.0** or later (Apple silicon & Intel).

## Auto-update

Installed copies check `releases/latest/download/appcast.xml` and offer new versions inside the app — no manual reinstall. Updates are verified with an EdDSA signature before they are applied.

## What's in this repo

Distribution artifacts only:

- **`Maestro.dmg`** — the signed, notarized disk image (one per release tag).
- **`appcast.xml`** — the EdDSA-signed Sparkle feed. `releases/latest/download/appcast.xml` always resolves to the newest release.

The application source lives in a separate repository.
