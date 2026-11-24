---
title: Updates
description: Changelog for the Praxis iOS app — recent changes, fixes, and refinements
---

# Updates

A record of what's changed in Praxis since launch. Most updates ship as over-the-air changes — they reach your phone the next time you cold-launch the app with WiFi on, no App Store update required. Bigger ones, like Praxis 2.0, come through the App Store.

[Get Praxis on the App Store ↗](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714)

---

## {{RELEASE_DATE}} — Praxis 2.0

The biggest update since launch: your practices can now follow you to your iPad, your wrist and your Lock Screen. Unlike most updates on this page, this one comes through the App Store, and it needs iOS 17 or later.

### Added
- **iCloud sync between iPhone and iPad.** Turn on **Sync across devices** in Data & Storage, and your practices, history, areas and Flows stay in step on every device signed in to your Apple ID. It uses your own iCloud account, so there's still no Praxis account and no Praxis server. If you change a practice on one device and log it on another before they've synced, both are kept, and changing when a session happened updates it on every device, note included. Sync is part of the one-time unlock; exporting and restoring backups stays free.
- **Apple Watch.** The **Praxis Ring** complication shows how today (or this week) is going at a glance. Choose what it tracks and whether partial sessions count, from **Apple Watch** in the menu. Open the watch app to see what's due, log a practice with a tap, dial in a count or minutes with the Digital Crown, and pause, resume or finish a running timer from your wrist.
- **The watch tells you what's on it.** Its list holds every practice the ring tracks that's due today or overdue, plus the ones you've done today, up to 100, and **Apple Watch** in the menu says how many are on your wrist and why any are left off. After midnight the watch says **New day** until your iPhone sends the new list, so yesterday's practices never pass for today's.
- **Praxis on iPad.** It now runs natively on iPad, in any orientation.
- **Live Activities.** A running timer sits on your Lock Screen and in the Dynamic Island, so you can see how long you've been at it without opening the app. It has Pause and Done buttons, which work while Praxis is running in the background.
- **Nine widgets.** Up Next, Today's Progress, Life Balance, Daily Wisdom, Aura Focus, Aura Pulse, Chart, Quick Log and Command. Up Next, Today's Progress and Daily Wisdom also work on the Lock Screen. **Quick Log** lets you log a due practice with one tap from the Home Screen, **Chart** shows the practices you pick (set it up from **Chart widget** in the menu), and **Command** is a large dashboard for iPad.
- **Choose the days a practice applies to.** Weekday-only practices wait quietly under **Not today** on the weekend instead of turning overdue. Something you last did on Friday reads as due on Monday, not three days late, because the days off were never meant to count.
- **Reminders for individual practices.** Turn on a reminder in a practice's details and pick a time. It arrives on the day the practice is due, skips days you've already done it, and tapping it brings that practice to the top of Focus.
- **An optional next due date.** For things tied to the calendar, like trash day, set the date it's next due and Praxis keeps it on that fixed schedule. Taking the bins out a night early no longer quietly moves trash day.
- **Background timers: several at once, and pausable.** Laundry, a slow cook and a fast can all run together, each with its own card and Live Activity. Pausing one also holds its "target reached" notification until you resume.
- **Running timers stay at the top of Focus.** Active practices pin above the list so they're always easy to find, and fold into compact rows as you scroll when several are going.
- **Swipe a practice on Focus to edit it or open its stats.** Tapping a card used to lead nowhere; now a swipe gets you straight to the two things you most often want.
- **A Difficulty tab in practice stats.** If you rate sessions, see how they've felt over time, with a period selector to zoom in or out.
- **The session-length curve reaches everyone.** The smooth distribution curve described in the August 2 entry below is part of 2.0, so App Store users get it now too.
- **A much bigger, searchable set of practice icons.** About 130 icons in categories like Movement, Mind, Home and Outdoors, with search, so every practice can have an icon that fits.
- **Colors for your areas and practice types.** Give each life area and practice type its own color, or leave it on **Auto**, which picks a calm color and keeps it when you add or reorder areas. A practice takes its area's color, Home gets one of its own, and the colors show next to names, on the Focus filter chips and in Stats, so your areas are easy to tell apart at a glance. Choose one by tapping **Edit** on an area in the Areas tab, or **Type settings** in a practice's details.
- **Set the time of day on sessions you add by hand.** Past entries used to be pinned to noon, which skewed time-of-day patterns. Now you pick when it actually happened.
- **Counts in completion history.** For practices with a daily count, each logged entry shows how many (for example "12×"), the same way timed sessions show minutes.
- **Insights keep their history.** New insights are marked **New** and sorted to the top, and earlier ones you haven't dismissed stay in the list instead of disappearing when a fresh batch arrives.
- **Crash reports can be turned off.** Praxis sends crash and freeze reports, with some basic app-health information, to Sentry so problems can be found and fixed. They never include your practices, notes or ratings. If you'd rather not send them, open the menu, tap **Settings**, and turn off **Send crash reports** under **Privacy**. The choice applies to the device you change it on.
- **Tap the tab you're on to scroll back to the top.** Works on all five tabs, the way most iPhone apps do.

### Changed
- **The unlock now includes iCloud sync.** The free version still includes up to 5 practices, 2 life areas, 4 rooms, 2 zones and 1 Flow, along with widgets, the watch app, Live Activities, insight cards and backups. The one-time unlock still removes those limits, and now adds iCloud sync. Still no subscription.
- **Lumen has been retired.** Lumen, the optional on-device assistant that came with the one-time unlock, isn't part of Praxis 2.0. The insight cards it used to explain stay, and they're free. If you downloaded Lumen's model, updating deletes it and gives you back about 1.9 GB of storage, and Praxis shows a short note once to say so. Your practices, history and notes aren't touched. If a device stays on Praxis 1.5, Lumen keeps working there.
- **One ring for today after you log a practice.** The completion screen now shows a single ring for how today is going ("3 of 5 today"), with a tag for the area you just logged. It replaces a set of nested, unlabeled rings whose colors came from their place in the list and were easy to mistake for statuses. An unfinished ring stays your theme's calm color, never red, and each day starts fresh.
- **One way of counting "today", everywhere.** The completion ring, the Focus header, the Today's Progress widget, the Lock Screen ring and the Apple Watch ring all count the practices due today or overdue, plus what you've done today. They always agree unless you've changed what the Praxis Ring tracks (from **Apple Watch** in the menu); then the watch and Lock Screen rings count just what you chose. "This week" means the last seven days everywhere too. Green, yellow, orange and red describe how your practices are doing, not today's progress, which has its own color.
- **Insight cards are calmer.** Cards describe your rhythm in plain numbers, without words like "slipping" or "never completed on time". The card that said one miss often leads to another is gone, and so is the one that counted a run of on-time sessions, because Praxis doesn't keep score of streaks. When a practice's target and your actual rhythm have drifted apart, you see one card with a suggested target instead of two. Cards already on your phone switch to the new wording.
- **Notification titles drop the flame.** iOS already shows the Praxis icon, and a flame at the start of a daily reminder reads like a streak alert. The daily check-in is now simply called "Daily check-in".
- **The Practices tab is now a plain management list.** Status colors live on Focus, where you decide what to do today. Practices is where you set things up, so its rows show each practice's name, place and schedule without urgency color. Swipe to delete still works.
- **Logging a practice with a daily count now starts at 1.** In the spring the completion dialog began defaulting to your full daily target, which over-logged single sessions: one set of pushups could read as the whole day. It now starts at 1, with a box for a larger batch.
- **Rooms belong to a life area.** The layout is now life area, then an optional zone, then room, and adding a room asks which area it's in. That keeps every room findable when you pick a place for a practice.
- **Praxis 2.0 needs iOS 17 or later.** iOS 17 is what lets widgets and Live Activities have buttons, so everyone on 2.0 gets one-tap Quick Log and the Pause and Done buttons on a running timer. The iPhone 8, iPhone 8 Plus and iPhone X, the iPad (5th generation), and the 9.7-inch and first 12.9-inch iPad Pro can't update to iOS 17. If you already have Praxis on one of them, you keep Praxis 1.5 as it is, but Praxis can no longer be newly installed there.

### Fixed
- **Unlock and Restore recover if the App Store was unreachable at launch.** If Praxis couldn't reach the App Store when it opened, tapping Unlock or Restore used to fail until you restarted the app. Now it tries again when you tap. Backing out of the purchase sheet no longer shows an error, and the unlock screen no longer shows an empty price when the price couldn't load.
- **Rooms without a zone could go missing from the room picker.** A room saved without a zone wasn't connected to any life area, so it never showed up when choosing a room for a practice. Rooms now carry their area directly, and older rooms with neither an area nor a zone appear under every area, so nothing is stranded.
- **Focus filters show your practices straight away.** Picking a Type, Area, Zone or Room filter before choosing how much time you had left the "How much time do you have?" question on screen, which looked like an empty list. A filter now shows the matching practices right away, and when nothing matches, Focus says so and offers **Clear filters**.

## 2026-08-02

### Added
- **Your session lengths now read as a smooth shape, not just bars.** The Time tab's distribution chart can draw a curve through your sessions instead of a bar chart — easier to see at a glance where your sessions actually cluster and how long the tail runs. A Curve / Both / Bars toggle sits on the chart and remembers what you picked. Under the curve is a small tick for every session you've logged, so you can always see how much history the shape is built from.
- **A plain-English read of the chart.** Under the curve: "Most sessions land near 27 min. Half fall between 21 and 35 min. Nine in ten are under 54 min." Those numbers come straight from your own sessions.
- **The chart declines to draw a shape it can't support.** With only a handful of sessions logged you'll see the individual sessions rather than a confident-looking curve drawn through almost no data — a smooth line looks just as sure of itself at nine sessions as at ninety, and that would be misleading. If you log durations by tapping the round-number chips (5, 10, 15, 20…), the chart shows those exact values as marks instead of pretending to a precision the numbers don't have.

### Fixed
- **The "previous period" series in Compare mode was grey instead of its own colour.** It was meant to be a clearly distinct colour from the current period, but was quietly falling back to the same muted grey as ordinary text — which also affected the legend swatches and, on shared practices, the bars for other people in the household chart. It now gets its own colour, and stays grey on themes where that colour would be too close to the accent to tell apart.

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
