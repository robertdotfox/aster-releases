# Aster releases

Public download point for **Aster**, a conversation companion designed for
presence over engagement.

The Aster source code is private; this repo exists only to host signed,
notarized release builds so [Sparkle](https://sparkle-project.org/) on
recipients' Macs can auto-update.

## Download

[**↓ Aster (latest .dmg)**](https://github.com/robertdotfox/aster-releases/releases/latest/download/Aster.dmg)

That link always resolves to the most recent release — no need to dig
into the Releases tab. Same for the appcast Sparkle reads:
[`appcast.xml`](https://github.com/robertdotfox/aster-releases/releases/latest/download/appcast.xml).

## Install

1. Download `Aster.dmg`.
2. Open it, drag Aster into Applications, eject the DMG.
3. Double-click Aster. Gatekeeper sees it's signed + notarized; no warning.
4. On first launch Aster walks you through installing
   [Claude Code](https://docs.anthropic.com/en/docs/claude-code/quickstart),
   which it uses for inference. Roughly:
   ```
   npm install -g @anthropic-ai/claude-code
   claude          # sign in once
   ```
5. Click "I've installed it — re-check" in Aster's onboarding panel and you're in.

Recipient needs: an Apple Silicon Mac, macOS 26 (Tahoe) or later, Node.js,
and an Anthropic account (Claude Pro/Max or API).

## Auto-update

Aster polls this repo's `appcast.xml` automatically. New versions are
verified against an EdDSA signature embedded in the app — only updates
signed by the developer's private key will install.

If you want to check manually: Aster menu → Check for Updates… (or ⌘⇧U).

## All releases

Browse every published version at the [Releases tab](https://github.com/robertdotfox/aster-releases/releases).

## Contact

Found a bug, voice drift, or feedback: robertdotfox@gmail.com
