# Loquen updates

This repository exists for one reason: to serve the Sparkle appcast that
[Loquen](https://github.com/neilbdesai) checks for updates, and to hold the signed,
notarized disk images it downloads.

- `appcast.xml` — the update feed, served over HTTPS by GitHub Pages at
  <https://neilbdesai.github.io/loquen-releases/appcast.xml>. Every entry is signed with an
  EdDSA key whose public half is compiled into the app; a tampered download will not install.
- **Releases** — one per version, each with a `Loquen-<version>.dmg`.

**To install Loquen:** open the [latest release](https://github.com/neilbdesai/loquen-releases/releases/latest),
download the DMG, and drag Loquen to Applications. After that the app updates itself.

The application source is not here.

## About the 0.1.x releases

Loquen was called Sotto until 2026-09-06. The `v0.1.0`–`v0.1.2` releases below still carry
the old name and are kept for the record. The feed is deliberately empty of them: a Loquen
build must never be offered a Sotto disk image. The first Loquen release repopulates it.
