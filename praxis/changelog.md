---
title: Updates
description: Changelog for the Praxis iOS app — recent changes, fixes, and refinements
---

# Updates

A record of what's changed in Praxis since launch. Updates ship as over-the-air changes — most of them reach your phone the next time you cold-launch the app with WiFi on, no App Store update required.

[Get Praxis on the App Store ↗](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714)

---

## 2026-05-10

### Added
- **Two new practice toggles: "Runs in the background" and "Has target duration."** The old "Long-duration practice" toggle conflated two unrelated things — whether a timer runs in parallel with another practice, and whether it should fire a notification when the duration is reached. Splitting them lets you mark "Do Laundry" as a background practice without it pestering you with a "target reached" notification (its 1-hour estimate is informational, not a goal). Fasting practices and other goal-oriented durations turn both toggles on. Notifications now only fire for practices you've explicitly marked as having a target duration.
- **Symmetric collision alerts.** Trying to start a second active practice while one is timing now reads *"Active practice in progress: <name> is already running. Finish or end it before starting another."* Same shape as the existing background-practice alert, both reference the offending practice by name.

### Changed
- **Unified timer display to hh:mm:ss across all practices.** Active timers used to show MM:SS (e.g. `01:30`), background timers used to show "Nh MMm" (e.g. `0h 02m`). One consistent format means a 90-second timer and a 4-hour fast read identically — `00:01:30` and `04:00:00`.

### Fixed
- **Long-duration practice timer no longer says "End Fast."** Long-duration practices include fasting but also things like laundry, slow cooking, sleep tracking, and any other practice you'd time over hours instead of minutes. The button now says "Done" (matching short-duration practices), and the header subtitle says "Timing: <name>" instead of "Fasting: <name>." User-reported via the Do Laundry practice.
- **Fixed a crash path in icon-theme syncing.** On iOS 26.3.1 a small number of devices saw an unhandled error when the home-screen icon tried to update for a theme switch. The icon sync is best-effort cosmetic — the fix wraps it so it can never crash, and falls back silently if the platform doesn't have the relevant alternate icons available.

## 2026-05-09

### Added
- **Tab-based filters on the Focus screen.** Narrow your list by Type, Area, Zone, or Room. Tap a filter tab to see options; selections combine across tabs ("Health area + 30 minutes," "Cleaning type + Kitchen room," etc.). Time and filters share the same tab bar; Time is the default.
- **[Public sources page](sources)** listing every classical quote and every frequency recommendation in the app, with links to primary sources. Linked from the bottom of the About screen.
- **This page.** Public changelog at [praxis/changelog](changelog) — recent updates and changes since launch. Linked from the bottom of the About screen alongside the Sources link.
- **Tap the version footer in the menu** to open this changelog. ("View recent changes" link added under the version + OTA info.) Long-press still shows the diagnostic info with an option to share for support emails.

### Changed
- **Replaced apocryphal classical quotes** in the practice-completion screen with verified passages from primary sources. The Confucius "go slowly" line isn't actually in the *Analects*; the Buddha "do not dwell on the past" quote isn't in the Pali Canon. Replaced both with real passages — Confucius's *"Learning without thinking is labor lost"* (Analects 2.15) and the Buddha's *Bhaddekaratta Sutta* (Majjhima Nikaya 131). Corrected a few Marcus Aurelius and Epictetus attributions while we were at it.
- **Corrected several frequency recommendations** to point to verified research instead of widely-cited-but-unsupported claims. The "reading 6 minutes reduces stress 68%" stat, for example, was a 2009 marketing-funded press release, not a peer-reviewed study — replaced with the Bavishi *et al.* 2016 longevity research. Similar corrections for several other recommendations; full list on the [sources page](sources).

## 2026-05-07

### Added
- **Log a practice anyway when the timing window says "too soon."** Tap Begin or Done on a too-soon practice and a confirmation dialog appears: *"This practice has not passed the min frequency yet — log anyway?"* Useful for special circumstances — a second shower in a heat wave, mopping the floor again after a spill, an unplanned workout because you're feeling great.

### Launched
- **Praxis v1.0 went live on the App Store.** Free to try, with a one-time $9.99 unlock after about two weeks of regular use. No subscription, no account, no servers. iPhone only for v1.0; Android and iPad come later.

---

Have a question about a specific change, or noticed something that doesn't look right? Email **praxis.app.support@gmail.com**.

— Matt Peterson
