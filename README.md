# homebrew-tap

Homebrew tap for [MD-Memo](https://github.com/youshinh/md-memo), a fast Markdown scratchpad with AI built in.

```bash
brew install --cask youshinh/tap/md-memo
```

Upgrade with `brew upgrade --cask md-memo`. Requires macOS 10.15 or later; the build is universal (Apple Silicon and Intel).

## First launch

The app is ad-hoc signed, not notarized by Apple, so macOS blocks it the first time.

- **macOS 15 (Sequoia) or later:** click *Done* in the dialog, open *System Settings > Privacy & Security*, scroll to *Security* and click *Open Anyway* (shown for about an hour after the attempt).
- **macOS 14 or earlier:** right-click the app in Finder and choose *Open*.
- **Any version:** `xattr -dr com.apple.quarantine /Applications/MD-Memo.app`

## About this repository

`Casks/md-memo.rb` is a copy of [`packaging/homebrew/md-memo.rb`](https://github.com/youshinh/md-memo/blob/main/packaging/homebrew/md-memo.rb) in the main repository, updated after each release (`version` and `sha256` must match the release's `md-memo-macos.zip`).
