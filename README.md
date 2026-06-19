# The Aster Codex

The writings the app rests on. Two books are shared publicly.

### [Book I — The Heart of Aster](./codex/Book%20I%20%E2%80%94%20The%20Heart%20of%20Aster.md)

The philosophical foundation. What wisdom is, why it cannot be given,
and why Aster is built as a companion rather than an authority. If you
want to know what Aster *is for*, start here.

### [Book V — The Journey of Becoming](./codex/Book%20V%20%E2%80%94%20The%20Journey%20of%20Becoming.md)

The lived version. Twelve chapters on conditions every person meets —
stillness, fear, resistance, honesty, courage, suffering, identity,
self-trust, change, love, meaning, flourishing — each paired with a
conversation showing what participation actually looks like. If you
want to know what *talking with Aster feels like*, read a chapter.

---

# Aster releases

Public download point for **Aster**, a conversation companion designed for
presence over engagement.

> 📖 **[Read what Aster is before you install →](WELCOME.md)**
> A one-page intro to how Aster works and how to talk to it.

The Aster source code is private; this repo exists only to host signed,
notarized release builds so [Sparkle](https://sparkle-project.org/) on
recipients' Macs can auto-update.

## Download

[**↓ Aster (latest .dmg)**](https://github.com/robertdotfox/aster-releases/releases/latest/download/Aster.dmg)

That link always resolves to the most recent release — no need to dig
into the Releases tab. Same for the appcast Sparkle reads:
[`appcast.xml`](https://github.com/robertdotfox/aster-releases/releases/latest/download/appcast.xml).

## iOS (TestFlight beta)

[**↓ Join the Aster iOS beta on TestFlight**](https://testflight.apple.com/join/ApdCzTSy)

On your iPhone: install the free [TestFlight app](https://apps.apple.com/app/testflight/id899247664)
if you don't have it, tap the link above, then tap **Accept** to start
testing. New builds notify you automatically in TestFlight.

## Install

1. Download `Aster.dmg`.
2. Open it, drag Aster into Applications, eject the DMG.
3. Double-click Aster. Gatekeeper sees it's signed + notarized; no warning.
4. On first launch Aster walks you through installing
   [Claude Code](https://docs.anthropic.com/en/docs/claude-code/quickstart),
   which it uses for inference. Roughly:
   ```
   curl -fsSL https://claude.ai/install.sh | bash
   echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc && source ~/.zshrc
   claude          # sign in once
   ```
5. Click "I've installed it — re-check" in Aster's onboarding panel and you're in.

Recipient needs: an Apple Silicon Mac, macOS 26 (Tahoe) or later, and an
Anthropic account (Claude Pro/Max or API). The install script puts the
`claude` binary in `~/.local/bin/`; the second line adds that directory
to your PATH and reloads the current shell so `claude` is immediately
runnable. No Node.js required.

## Auto-update

Aster polls this repo's `appcast.xml` automatically. New versions are
verified against an EdDSA signature embedded in the app — only updates
signed by the developer's private key will install.

If you want to check manually: Aster menu → Check for Updates… (or ⌘⇧U).

## All releases

Browse every published version at the [Releases tab](https://github.com/robertdotfox/aster-releases/releases).

## Contact

Found a bug, voice drift, or feedback: robertdotfox@gmail.com
