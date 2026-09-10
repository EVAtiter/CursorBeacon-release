[日本語](README.md) | **English**

# CursorBeacon

**Hold down the fn key (or the right Option key) and you will know where your mouse cursor is.**

On a large display or a multi-monitor desk, when you cannot tell where the pointer went,
just hold the key for 0.3 seconds: **everything dims except the area around your cursor**,
and a glowing red octagonal field unfolds there. Let go and everything returns to normal.

## There are two editions

CursorBeacon is distributed through two channels. **Their features differ slightly.**

|  | Mac App Store | Direct download |
|---|---|---|
| Where to get it | [Mac App Store](https://apps.apple.com/app/cursorbeacon/id6808957431) | GitHub Releases / Homebrew |
| **Spotlight (dimming)** | **Yes** | **Yes** |
| **Glowing octagonal field** | **Yes** | **Yes** |
| Special permissions | Not required | Not required |
| Price | Free | Free |
| Magnifying the cursor itself | — | Yes (smoothly, up to 3×) |
| Hiding the menu bar icon | — | Yes |
| App Sandbox | Yes | No (Developer ID signed and notarized by Apple) |

> **Spotlight and the octagonal field — the core of how CursorBeacon points out your cursor —
> are in both editions.** The direct download edition magnifies the cursor itself on top of that.
>
> **Why they differ:** changing the size of the cursor requires a private macOS interface that
> App Store rules do not permit. **Neither edition requires any special permission.**

## Features (in both editions)

- **Press, and you find it** — no shaking the mouse around, no hunting across screens
- **Three triggers** — the fn key, the right Option key, and the **left Control key**
  (since v1.3.0, off by default). "Additional Hot Keys" in the menu switches the right
  Option and left Control keys on or off individually (**the fn key always works**, so
  turning both off still leaves you a trigger)
- **Spotlight** — everything but your cursor's surroundings goes dark, so the position is
  obvious at a glance (can be turned off from the menu)
- **Never in your way** — clicks go straight through to the app underneath while the screen
  is dimmed
- **Works across displays** — every screen dims, leaving only the cursor's position lit
- **Hard to set off by accident** — the left Option key and the right Control key do
  nothing, and neither do held arrow or function keys. If you click, drag or press a shortcut while holding the trigger,
  it stops immediately
- **No special permissions** — neither Accessibility nor Input Monitoring is needed
- **Lives in the menu bar** — can start automatically at login

## Installation

### Mac App Store edition

https://apps.apple.com/app/cursorbeacon/id6808957431

### Direct download edition

#### Homebrew

```
brew install --cask EVAtiter/tap/cursorbeacon
```

#### Manually

Download the latest `CursorBeacon-<version>.zip` from
[Releases](https://github.com/EVAtiter/CursorBeacon-release/releases), unzip it, and move
`CursorBeacon.app` into your Applications folder.

## How to use

1. Launch the app (a pointer icon appears in the menu bar)
2. **Hold the fn key, the right Option key, or the left Control key for 0.3 seconds
   or longer** (the left Control key is off by default; enable it under
   "Additional Hot Keys" in the menu)
3. Release the key and everything returns to normal

Turn on "Open at Login" from the menu bar icon and you will not have to think about
starting it again.

## Uninstalling

### Mac App Store edition

Move `CursorBeacon.app` from your Applications folder to the Trash.

### Direct download edition

If you installed it with Homebrew:

```
brew uninstall --cask cursorbeacon
```

If you installed it manually, move `CursorBeacon.app` from your Applications folder to the
Trash. The login item can be removed under System Settings → General → Login Items.

## Requirements

- macOS 13.0 (Ventura) or later
- **Apple Silicon (arm64) only** (it does not run on Intel Macs)

## Support

Please report bugs and feature requests as Issues.

🔗 https://github.com/EVAtiter/CursorBeacon-release/issues

## Privacy Policy

This application collects and transmits no data of any kind.

🔗 [Privacy Policy (English)](PRIVACY.md) / [プライバシーポリシー（日本語）](PRIVACY.ja.md)

---

Copyright © 2026 EVA Titer. All rights reserved.
