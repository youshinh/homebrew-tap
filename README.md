# homebrew-tap

Homebrew tap for [syki::sok](https://github.com/youshinh/syki-sok), a zero-latency, local-first Markdown scratchpad engineered for instant capture, with optional AI features.

```bash
brew install --cask youshinh/tap/syki
```

Upgrade with `brew upgrade --cask syki`. Universal binary (Apple Silicon and Intel).

## First launch

The app is ad-hoc signed, not notarized by Apple, so macOS blocks it the first time.

- **macOS 15 (Sequoia) or later:** click *Done* in the dialog, open *System Settings > Privacy & Security*, scroll to *Security* and click *Open Anyway* (shown for about an hour after the attempt).
- **macOS 14 or earlier:** right-click the app in Finder and choose *Open*.
- **Any version:** `xattr -dr com.apple.quarantine /Applications/syki-sok.app`

## About this repository

`Casks/syki.rb` is a copy of [`packaging/homebrew/syki.rb`](https://github.com/youshinh/syki-sok/blob/main/packaging/homebrew/syki.rb) in the main repository, updated after each release.
