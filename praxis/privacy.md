---
title: Privacy Policy
description: Privacy Policy for Praxis on iPhone, iPad and Apple Watch
---

# Privacy Policy for Praxis

**Effective: {{EFFECTIVE_DATE}}**

Praxis is a practice tracker for iPhone, iPad and Apple Watch, built by Matt Peterson. This page explains what information Praxis handles, where it goes, and the choices you have. It applies to every version of Praxis. Some of what it describes arrived in Praxis 2.0: iCloud sync, the Apple Watch app, widgets, Live Activities, practice reminders and the switch for turning crash reports off. The parts about those apply from version 2.0. Lumen, which Praxis 2.0 removes, has its own section for anyone still using Praxis 1.5.

[Get Praxis on the App Store ↗](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714)

## The short version

- **Praxis has no servers of its own and no accounts.** There is nothing to sign up for.
- **Your practices live on your devices.** If you turn on iCloud sync, they are also stored in your own iCloud account. We can't see any of it.
- **Two services receive limited technical information, never your practice content:** Sentry, for crash and freeze reports, and Expo, which delivers app updates. From Praxis 2.0, you can turn crash reports off inside the app.
- **No ads and no tracking.** Praxis doesn't track you across other apps or websites, and your information is never sold.

## What Praxis stores on your devices

Praxis keeps its data in the app's own storage on each device you use it on:

- Your practices and their settings: schedule, targets, reminders, icons
- Your life areas, zones, rooms, practice types, Flows and links, including any colors you pick for areas and types
- Your completion history, including durations, counts, and any notes and ratings you add
- Themes, design choices and app settings
- The insight cards Praxis works out from your history

This data stays on the device except in the ways described below, or when you export a backup yourself from **Data & Storage**.

### On your Lock Screen, Home Screen and Apple Watch

Some of this information appears outside the app, where anyone holding your device can see it without unlocking it:

- **Widgets** show practice names and progress on your Home Screen, and some can be placed on your Lock Screen.
- **Live Activities** show the name of a running practice and its timer on your Lock Screen and in the Dynamic Island.
- **Notifications** for practice reminders and timer targets show the practice's name.
- **The Apple Watch app and the Praxis Ring complication** show practice names, progress and running timers.

To put that information there, Praxis shares it with its own widget extension on the same device, and sends it directly between your iPhone and your paired Apple Watch using Apple's WatchConnectivity. None of it passes through a server of ours. If you'd rather keep it off the Lock Screen, remove the widgets, turn off Live Activities for Praxis in iOS Settings, or change notification previews in iOS Settings → Notifications.

## iCloud sync (optional)

iCloud sync is off until you turn it on in **Data & Storage → Sync across devices**. It is part of the one-time unlock.

**What syncs.** Your practices and their completion history (including notes and ratings), your life areas, zones, rooms and practice types (with any colors you picked), and your links and Flows. Praxis also keeps a short list of your devices in the same place: a random identifier, whether it's an iPhone or iPad, and when it last synced. Settings, themes and insights stay on each device.

**Where it lives.** In your private iCloud account, in two places: a data file in the Praxis folder of iCloud Drive (you can see it in the Files app under iCloud Drive → Praxis), and a private CloudKit database. Apple stores this data under [Apple's Privacy Policy](https://www.apple.com/legal/privacy/) and the iCloud terms. We have no access to your iCloud account or anything in it.

**Turning sync off** stops syncing. It doesn't delete anything already in iCloud, and each device keeps its own copy.

**Deleting your Praxis data from iCloud:**

1. Turn off **Sync across devices** on every device that uses it. Otherwise another device will upload the data again.
2. On your iPhone or iPad, open **Settings → [your name] → iCloud → Manage Account Storage** (called **Storage** on some iOS versions) → **Praxis**, and choose to delete its data. Deleting the file in the Files app isn't enough on its own: it removes only that file, not the copy in the CloudKit database, so use Settings for a full delete.

Your data stays on each device after this, until you delete it there too.

## Lumen (Praxis 1.5 and earlier)

Praxis 1.5 and earlier include Lumen, an optional assistant that explains the patterns in your practice. It runs entirely on your device, using Llama 3.2 3B, a small language model.

- **An optional download.** The model file (about 1.9 GB) is downloaded from Hugging Face only if you choose to download it inside Lumen. Like any download, Hugging Face receives the request itself, including your IP address. Only the model is downloaded. Nothing about you, your practices or your usage is sent. If you never download it, Praxis never contacts Hugging Face.
- **Everything else happens on your device.** The prompts you tap, your data and Lumen's answers never leave it.

**Praxis 2.0 removes Lumen.** When you update, Praxis deletes the downloaded model file and the insights Lumen saved, which frees about 1.9 GB if you had downloaded it. Your practices and history aren't touched, and the insight cards stay. Praxis 2.0 doesn't download or contain a language model.

**Built with Llama.** Lumen is built with Llama. Llama 3.2 is licensed under the Llama 3.2 Community License, Copyright © Meta Platforms, Inc. All Rights Reserved. [Read the Llama 3.2 Community License ↗](https://github.com/meta-llama/llama-models/blob/main/models/llama3_2/LICENSE)

## Crash and freeze reports (Sentry)

Praxis uses [Sentry](https://sentry.io/privacy/), a third-party error-reporting service, to find and fix bugs. Sentry receives:

- **Reports when Praxis crashes or freezes,** describing the technical error and where in the app's code it happened
- **Basic session health,** meaning whether a session ended normally or with a crash
- **Your device model, iOS version, and Praxis version and build**
- **A random identifier created when Praxis is installed,** so reports from the same installation can be grouped. It isn't linked to your name, Apple ID or email.
- **Technical breadcrumbs,** a short trail of recent app events such as which screen was open or which on-screen control was tapped, to help reproduce a problem

Reports never include your practice names, notes, ratings or iCloud data. Praxis asks Sentry not to collect your IP address. Sentry is also set to store neither your IP address nor the approximate location (city, region and country) that it could otherwise work out from your connection. Sentry processes reports on its servers in the United States and keeps them for up to 90 days. Reports are used only to fix problems in Praxis.

**Turning crash reports off.** In Praxis 2.0 and later, open the menu (the button in the top-right corner), tap **Settings**, and turn off **Send crash reports** in the **Privacy** section. The choice applies to the device you change it on. Turning it off stops new reports straight away; anything already waiting to be sent may still finish sending, and a report saved on the device stays unsent unless you turn reports back on. Turning them back on takes effect after Praxis is fully closed and reopened. The switch covers Sentry only: Praxis still checks Expo for app updates, as described below.

## App updates (Expo)

Some fixes and improvements reach Praxis as over-the-air updates, delivered through [Expo](https://expo.dev/privacy). When Praxis launches, it checks Expo's servers for an update. The request includes the app version, the platform, the update channel and a random identifier created for this installation, which isn't tied to you. As with any internet request, Expo can see your device's IP address. No practice data is included.

## Purchases

Apple handles the Praxis in-app purchase. Apple receives your purchase details under its own privacy policy. Praxis checks your purchase with the App Store on your device and remembers the unlock on the device. We receive only aggregate sales reports from Apple and never see your payment information or Apple ID.

## Notifications

Notifications are optional, and iOS asks for your permission first. Every Praxis notification is created and scheduled on your device. None is sent from a server, and Praxis doesn't use push notifications. Praxis can send:

- **A daily check-in,** if you turn it on in the menu → **Settings → Notifications**
- **Practice reminders,** for practices where you turn on a reminder. The notification's title is the practice name.
- **Target reached,** when a timed practice with a target duration reaches it. It names the practice.
- **New insights,** when Praxis notices new patterns in your history

## Your choices

- **Keep everything on one device.** iCloud sync is off unless you turn it on.
- **Turn iCloud sync on or off** at any time, and delete the iCloud copy as described above.
- **Turn notifications off** in Praxis, per practice, or in iOS Settings → Notifications → Praxis.
- **Keep things off your Lock Screen** by removing widgets or turning off Live Activities for Praxis in iOS Settings.
- **Turn crash reports off** on each device where you want them off: in Praxis, open the menu, then **Settings**, and turn off **Send crash reports** under **Privacy** (Praxis 2.0 and later).
- **On Praxis 1.5, skip Lumen.** Nothing is downloaded unless you choose to.
- **Take your data with you.** Export a full backup any time from **Data & Storage → Export JSON** or **Export to Excel**.
- **Erase Praxis data on a device** with **Data & Storage → Reset All Data**, or by deleting the app. Resetting doesn't delete your iCloud copy; see above for that.

## Children

Praxis is not directed at children under 13, and we don't knowingly collect personal information from children.

## Changes to this policy

If we change how Praxis handles data, we'll update this page and change the effective date above. Significant changes will also be noted on the [Praxis updates page](changelog). Sharing practices with the people you live with is planned for a later version; this page will describe it before that version is released.

## Contact

Questions about your privacy or this policy? Email **praxis.app.support@gmail.com**.
