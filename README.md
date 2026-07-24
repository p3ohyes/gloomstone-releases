# Gloomstone — downloads & updates

Official Windows installers for **Gloomstone**, plus the two small text files the
game uses to keep itself up to date. The game's source code is private — only the
built installer and its update metadata live here, and everything in this repo is
readable.

## Get the game

Download the latest **`Gloomstone-Setup-x.y.z.exe`** from the
[**Releases**](../../releases/latest) page. After the first install the game updates
itself automatically, so you only download once.

Windows SmartScreen may warn that the installer is unrecognized — it isn't
code-signed yet, which is normal for a small indie build. Choose **More info → Run
anyway**, or verify the file's SHA-512 against the value listed in `latest.yml`.

## What the other files are

- **`latest.yml`** — tells an installed copy which version is newest, so it can
  update itself.
- **`blocklist.json`** — a small safety list. If a released build turns out to crash
  on launch, its version number can be added here so copies of *that specific broken
  build* show a "please update" message instead of launching into the crash. It is
  **normally empty** (as it is right now), it only ever names a version that already
  has a fixed replacement available, and if the file is ever missing or unreachable
  the game simply launches as usual. It cannot disable a working version, and it
  collects nothing.

That's the whole repository: one installer and two tiny text files.
