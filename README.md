# homebrew-alttab-rs

Homebrew tap for [AltTab-rs](https://github.com/jimbo23/alttab-rs), a native Rust rebuild of the
[AltTab](https://github.com/lwouis/alt-tab-macos) window switcher for macOS.

```sh
brew install --cask jimbo23/alttab-rs/alttab-rs
```

or

```sh
brew tap jimbo23/alttab-rs
brew install --cask alttab-rs
```

## Notes

- **Unsigned app.** Release builds are ad-hoc signed, not Developer ID signed or notarized. If Gatekeeper
  blocks the app, install with `brew install --cask --no-quarantine jimbo23/alttab-rs/alttab-rs`, or run
  `xattr -dr com.apple.quarantine /Applications/AltTab-rs.app` after installing.
- **Permissions.** Grant **Accessibility** (required for switching/focusing windows) and **Screen Recording**
  (optional, for window thumbnails) in System Settings → Privacy & Security.
- Requires macOS 12 (Monterey) or later; universal binary (Apple Silicon + Intel).

## License

GPL-3.0-only. AltTab-rs is a derivative of AltTab by lwouis and contributors (GPL-3.0).
