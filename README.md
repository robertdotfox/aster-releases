# Aster releases

Public download point for **Aster**, a conversation companion.

The Aster source code is private; this repo exists only to host signed,
notarized release builds so [Sparkle](https://sparkle-project.org/) on
recipients' Macs can auto-update.

## Install

Grab the latest release: <https://github.com/robertdotfox/aster-releases/releases/latest>

Download `Aster.dmg`, open it, drag Aster into Applications, and double-click.
On first launch Aster will walk you through installing
[Claude Code](https://docs.anthropic.com/en/docs/claude-code/quickstart),
which it uses for inference.

## Auto-update

Aster checks this repo's releases automatically. New versions are
verified against an EdDSA signature embedded in the app — only updates
signed by the developer's private key will install.

## Contact

robertdotfox@gmail.com
