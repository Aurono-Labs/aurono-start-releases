# Aurono Start — Release artifacts
This repository hosts release artifacts for [Aurono Start](https://auronolabs.com) — built tarballs and checksums published when we cut a beta release. There is no source code here.

> **Aurono Start is currently in private beta.** If you landed here without prior contact from us, please [reach out via auronolabs.com](https://auronolabs.com) before installing — early-beta installs benefit from some hand-holding.

## What's in a release
Each release page attaches two files:

| File | Purpose |
|---|---|
| `aurono-start-X.Y.Z.tar.gz` | The release bundle (pre-built frontend, Python source, install scripts). |
| `aurono-start-X.Y.Z.tar.gz.sha256` | SHA-256 checksum of the bundle. Verify before install with `sha256sum -c` (Linux) or `shasum -a 256 -c` (macOS). |

> **About the "Source code" assets.**
Every GitHub release auto-generates "Source code (zip)" and "Source code (tar.gz)" download buttons. On this repository they only contain this README — they're a UI artifact, not the actual download. Use `aurono-start-*.tar.gz` for installs.

## Where the source code lives
Aurono Start's source code lives in a private repository during beta. Parts of it — the trust layer (strategy evaluation, decisions, ledger, events; the components that decide and execute trades) — will be open-sourced before general release.

## Updating an existing install
If you're a beta tester running v0.1.3-beta or newer, Aurono Start checks for new releases automatically and shows a banner on the Dashboard with a copy-paste install command when one's available. Aurono itself never downloads or runs the installer — you stay in control.
