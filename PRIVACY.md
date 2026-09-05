# Privacy Policy

**English** | [日本語](PRIVACY.ja.md)

Last updated: September 5, 2026

This policy applies to **CursorBeacon**, a macOS application developed by
EVA·Titer, in **both** of its editions:

- the **Mac App Store edition**, and
- the **direct download edition** distributed via GitHub Releases and Homebrew.

Everything below applies to both unless a section says otherwise.

---

## We do not collect any data

This application **does not collect, store, transmit, or share any personal
information or usage data whatsoever.**

Specifically:

- No analytics, telemetry, crash reporting, or usage tracking
- No advertising and no advertising identifiers
- No user accounts, sign-in, or registration
- No network communication of any kind — the application never connects to the
  internet or to any server operated by the developer or a third party
- No access to your contacts, calendars, photos, location, microphone, or camera

## About keyboard detection

The application reveals your cursor while you hold the fn key or the right
Option key. Because of what it does, we want to be explicit about what it does
**not** do.

The application only asks the operating system two things:

1. **Which modifier keys are currently held** (via `NSEvent.modifierFlags` and
   `CGEventSource.flagsState` / `keyState`)
2. **How many key presses, clicks, and scrolls have occurred in total** (via
   `CGEventSource.counterForEventType`), so that the effect can be cancelled
   the moment you start doing something else

The second one is a running count only. **The application never sees which keys
you type, nor the content of anything you enter.** It cannot: reading keystrokes
would require Input Monitoring or Accessibility permission, and this application
requests neither. Nothing about your keyboard activity is recorded or stored.

## Data stored on your Mac

The application saves your preferences — whether the Spotlight dimming is
enabled, and whether the app opens at login — locally on your Mac using the
standard macOS preferences system (`UserDefaults`).

This data never leaves your Mac. It is not accessible to the developer.
Removing the application and its preference file deletes it completely.

## Screen content

While the trigger key is held, the application draws a translucent overlay on
top of your screen. It **draws onto** the screen; it never reads, captures, or
records what is displayed. The application does not request Screen Recording
permission and cannot see the contents of your display.

## App Sandbox (Mac App Store edition)

The **Mac App Store edition** runs inside the macOS App Sandbox with no
additional entitlements. It cannot read your documents, access the network, or
use the camera or microphone — these capabilities are withheld at the operating
system level, not merely unused by our code.

The **direct download edition** is not sandboxed, because it uses a system
facility for resizing the cursor that is unavailable inside the sandbox. This
does not change what the application does: it still performs no network
communication, collects no data, and requests no privacy permissions. It is
signed with an Apple Developer ID and notarized by Apple.

## Third parties

This application contains no third-party SDKs, frameworks, or services.

## Changes to this policy

If this policy changes, the revised version will be published on this page with
an updated date. Because the application collects no data, any change is
expected to be clarifying rather than substantive.

## Contact

Questions about this policy can be raised as an issue in this repository:

https://github.com/EVAtiter/CursorBeacon-release/issues

---

Copyright © 2026 EVA·Titer. All rights reserved.
