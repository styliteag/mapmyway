---
title: Privacy Policy
description: MapMyWay privacy policy — your data stays on your device.
---

# MapMyWay Privacy Policy

[Support](support) · Contact: **wb@stylite.de**

**Effective date:** 2026-04-29

MapMyWay is a personal location tracker for iPhone. This policy describes what data the app uses, where it lives, and what we do with it. The short answer: your data stays on your device.

## What data the app uses

- **Location.** MapMyWay continuously reads your location (foreground and background) to record your daily movements. iOS asks you to grant "Always" permission. If you grant only "While Using", the app records only while it is open.
- **Motion.** MapMyWay reads CoreMotion data (accelerometer, pedometer) so the on-device activity classifier can tell walking from cycling, driving, and other movement types.
- **No account, no profile.** MapMyWay has no sign-in, no account system, and does not collect a name, email, phone number, or device identifier.
- **No analytics, no advertising, no third-party SDKs.**

## Where your data is stored

- **On your device.** All location samples, visits, trips, places, and activity classifications are stored in a local SQLite database inside the app's sandbox on your iPhone. Nothing is uploaded to a MapMyWay server — there is no MapMyWay server.
- **In your private iCloud Drive container** (only if iCloud is enabled on your device). The app writes daily route exports (GPX, optionally CSV) and weekly database backups to `iCloud Drive/MapMyWay/`. This is your private iCloud container under your Apple ID; only you can access it. Apple manages the storage. The developer of MapMyWay cannot read it.
- **Backup retention.** Database backups older than 90 days are automatically deleted from your iCloud container.

## Data we share with Apple

- **Map tiles and place lookups.** When MapMyWay shows a map or suggests names for places you have visited, it uses Apple's MapKit and Apple's local search. This sends coordinates to Apple under Apple's privacy policy. MapMyWay does not pass your data through any other server in between.

## Data we share with anyone else

None.

## Your control

- **Stop tracking.** Toggle off "Automatic Tracking" in Settings, or revoke the location permission in iOS Settings.
- **Delete your data.** Delete the app from your iPhone. The on-device database is removed with the app. To remove the iCloud copies, delete the `MapMyWay` folder in the Files app (iCloud Drive).
- **Export your data.** GPX and CSV files are written automatically to iCloud Drive in open formats; you own them and can move them anywhere.

## Children

MapMyWay is not directed at children and does not knowingly collect data from children under 13.

## Changes to this policy

If the way the app handles data changes, this page will be updated and the effective date above revised. Material changes will be reflected in the next App Store update notes.

## Contact

Questions or concerns: **wb@stylite.de**
