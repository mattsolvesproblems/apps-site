---
title: Updates
description: Changelog for the Praxis iOS app — recent changes, fixes, and refinements
---

# Updates

A record of what's changed in Praxis since launch. Updates ship as over-the-air changes — most of them reach your phone the next time you cold-launch the app with WiFi on, no App Store update required.

[Get Praxis on the App Store ↗](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714)

---

## 2026-06-10

### Fixed
- **Backups now include your Areas and Flows.** Since the May update that introduced life Areas, the JSON backup quietly left them out — restoring a backup brought all your practices back, but the areas you'd organized them into (and any Flows you'd built) were missing. Exports now save both. Importing an older backup made before this fix recovers gracefully too: practices are regrouped into their areas automatically, with placeholder names you can rename (the original names weren't saved inside those older files).
- **Restoring a backup right after "Reset all data" now sticks.** Resetting also cleared some internal bookkeeping, so if you imported a backup immediately afterward, the next launch could quietly reorganize everything back into just Home/Unassigned — undoing the restore. The app now recognizes restored data and leaves it alone.

## 2026-06-09

The "small consistent effort" model now applies to time-based goals, not just rep counts.

### Added
- **Time-target practices count partial sessions toward your daily goal.** If you aim to read 60 minutes a day and do two 30-minute sessions, they now add up to hit the goal — instead of the first session marking the whole day done. Same as how "25 pushups" already summed multiple logs, now applied to minutes.
- **"In rhythm" status for time goals.** Read 40 minutes yesterday toward a 60-minute goal and nothing yet today? The card reads "In rhythm" with "Recent: 40 min/day avg" instead of flagging you as overdue. Showing up below target is recognized, not penalized — and genuinely stopping for a week still surfaces normally.
- **Daily minutes chart.** The practice stats screen's "Durations" tab is now "Time," with a new "Daily" view showing total minutes per day against your target line — so you can see your daily-minutes trend the same way count practices show daily reps.
- **"Suggested target" for time goals.** If your reading sessions have settled at ~40 minutes over a few weeks when the goal says 60, a card offers to update the target to match — one tap, either direction (it'll also suggest raising the target if you've grown past it).

### Changed
- **Goal-oriented timed practices say "Target" instead of "Estimate."** When a practice has a real daily time goal (not just an informational duration like "Laundry ~60 min"), the stats screen now labels it "Target," "Change Target," and marks it "▼ target" on the distribution chart. Practices where the duration is just a rough estimate keep the "Estimate" wording.

### Added
- **"In progress" status for multi-log practices.** A "25 pushups daily" practice that you'd done 12 of used to still show a red "Must do" badge — looked like you hadn't done anything when you'd actually done about half. Now it shows a yellow "In progress" badge with "12/25 today" so you can see at a glance where you are.
- **"In rhythm" status for multi-log practices you're still doing, just below target.** Did 13 dips yesterday when your target is 20? Today's card now reads "In rhythm" yellow with "Recent: 14/day avg · yesterday" instead of "Very overdue" red. The system tracks engagement (any logged activity) as a separate signal from full-target completion — small consistent effort gets recognized, not penalized. Genuinely stopped doing something for a week or more still surfaces as "Must do" — the change is targeted, not blanket.
- **Counts chart tab for multi-log practices.** Same Stats screen that has Intervals and Durations now has a Counts tab — a daily-totals view of how many you've logged each day, with your target line overlaid. Compare mode works here too.
- **Compare mode on histograms.** Toggle to split your data in half (older vs newer) and see if your distribution is shifting — getting faster, more consistent, etc. Available on intervals, durations, and counts.
- **Setup wizard now starts with life areas.** Pick what matters to you (Home, Wellness, Mind, Personal Care, etc.) before drilling into specific rooms. The Rooms step only appears if you selected Home — non-spatial users skip it entirely. Sample data loaded into the wizard is now transparent: it shows you what's possible without counting against the free-tier cap.
- **New "Suggested target" insight card.** When your actual per-session count has settled at a different level than your stated target — say you've been doing ~15 dips per session for a month with low variance when the target is 20 — a card appears on the Stats > Insights tab offering to update the target to match what you're actually doing. One-tap "Update target to 15" button does it; "Keep at 20" dismisses. Either direction (lower or higher) — the system suggests raising the target when you've grown past it too.

### Changed
- **Free tier is now a cap on what you create**, instead of a time/usage threshold. You get **5 practices, 2 life areas, 4 rooms, 2 zones, and 1 Flow** on the free tier. If you already have more than that, you keep all of it — the cap only matters when you try to add more. Unlock removes all caps, and Lumen (the chat-style insights) is also part of the unlock. The rule-based insight cards remain free.
- **Lumen insights now use a deterministic detector engine** instead of running an on-device language model for the core narration. Validated against 5 real-world datasets — no false positives. Faster to generate (no model inference), more reliable, and easier to extend with new pattern types. The model still handles your text notes where genuine prose adds value.
- **Practice Details screen rearranged.** Sections (Where → What kind → Time & Logging → Frequency → Links → Season) with horizontal dividers and consistent spacing. Easier to scan for what you're trying to edit.
- **Picking a room no longer auto-appends its name to the practice name.** "Sweep" no longer becomes "Sweep Kitchen" when you select Kitchen. The room is rendered right next to the practice name on every card already, so the suffix was just clutter.
- **Sample practices are now preview-only on the free tier.** Loaded sample data shows everything you can do with the app — stats, charts, structure — but you can't edit names, frequencies, or completion entries until you unlock. Deleting samples is still allowed (it doesn't bypass anything).

### Fixed
- **Multi-log practices were saving count=1 even when you tapped Save on a full session.** A "20 pushups daily" practice you'd just done all of would record as "1 pushup logged" — so the day never hit target and the practice stayed flagged as never done. The completion dialog now defaults to your full target (the common case), with chips and a custom field for partial sessions. A one-time migration also recomputes the "last done" date on every existing practice so historical data heals itself.
- **Lumen no longer reports practices as "slipping" when you're actually doing them.** Tapping the "What's slipping?" chip used to surface multi-log practices you'd done partial sessions of (e.g. "Dips — last done 10 days ago" when you actually did 12 reps yesterday) because the system equated "below target" with "stopped doing." Now Lumen distinguishes the two: practices you're still engaging with daily but below target appear in a separate "showing up but below target" group with effort-aware copy. Practices you truly stopped doing for a week+ still surface as overdue.
- **Stale "last done" values after changing a practice's target.** Bumping a practice from "1× daily" to "2× daily" left the previous completion marker in place, so the practice could show "Too soon" even when you hadn't done the new amount. Fixed with the same migration above.
- **A handful of screens were silently freezing on certain taps.** Tapping "Ask Lumen" on a practice's stats modal, trying to edit a sample practice's frequency or duration, and the import wizard's overflow banner could all leave the app stuck. The unlock dialog now properly takes over instead of disappearing into iOS's modal stack. If you ran into one of these freezes, this update resolves it.
- **"Free tier full" on the setup wizard's Areas step right after a fresh reset.** A missing line in the reset flow was leaving the in-memory list of life areas intact. Fixed.
- **Histogram median markers were drifting from their true positions.** The triangle that marks your median value now sits at the right spot within its bin (proportional positioning), and axis labels show actual bin boundaries instead of bin centers — so the numbers match what you see.
- **"A little goes a long way" was clipping on Android.** The last word was getting cut off on some screen sizes. Fixed.

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
