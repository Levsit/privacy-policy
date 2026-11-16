# Privacy Policy — Phone Monitor – Device Health

**Effective date:** 16 November 2026 · [Version française](PRIVACY_POLICY.fr.md)

This policy explains what the Android app **Phone Monitor – Device Health**
(package `com.yan.phonemonitor`, "the app") does with information on your
phone. It is published by mezyan ("we").

## The short version

- Everything the app records **stays on your phone**.
- The app has **no internet access**: it does not request Android's
  `INTERNET` permission, so it cannot send anything anywhere.
- There are **no accounts, no ads, no analytics, no crash reporting** and no
  third-party tracking libraries.
- We **never see, collect, sell or share** your data.
- Android cloud backup and device-to-device transfer are **switched off** for
  the app, so its data is not copied to Google Drive or another phone.

## What the app reads, and why

The app is a device-health tool. To work, it reads information about your
phone from Android and stores the results in a local database on the phone.

| What | Why | Android permission or access |
|---|---|---|
| Battery level, charging state, temperature, voltage, current | Battery history, health, temperature warnings, "Last until" planner | None needed |
| Free and used storage, the size of each app (app, data, cache) | Storage history, "Free up space", biggest and fastest-growing apps | `PACKAGE_USAGE_STATS` (usage access) |
| Which apps were in the foreground and for how long, screen on/off, unlocks | Screen time, battery use per app, daily limits, recaps | `PACKAGE_USAGE_STATS` (usage access, which you switch on yourself) |
| Wi-Fi and mobile data used per app | Data usage, data limits, mobile data plan | `PACKAGE_USAGE_STATS`, and on Android 9 and older only `READ_PHONE_STATE` (needed there by Android's data-usage statistics; the app does not read your phone number, calls or device identifiers) |
| The list of installed apps, their names, icons and the permissions they hold | App list, permission review ("Permissions", "Privacy watch") | `QUERY_ALL_PACKAGES` |
| Which app is currently open | Enforcing the blocks, pauses, limits and schedules **you** set | Accessibility service "Phone Monitor app blocker" (you switch it on yourself) |
| Which app posted a notification | Muting the apps **you** choose, and counting how many notifications were silenced | Notification access "Phone Monitor notification muting" (you switch it on yourself) |

Notes on the two special accesses:

- **Accessibility service.** It only looks at the name of the app that comes
  to the foreground. It does not read what is on the screen, what you type,
  or any other content, and it does not perform actions for you except going
  to the home screen when a blocked app is opened. The app explains this and
  asks for your agreement before it sends you to the Accessibility settings.
- **Notification access.** It only looks at which app posted a notification.
  It does not read, store or show the title or text of any notification.
  Only counts (how many notifications from an app were silenced on a day)
  are kept.

The app also uses these permissions, which do not give it access to personal
data: notifications (`POST_NOTIFICATIONS`, to show warnings and recaps),
foreground service, wake lock and start at boot (to take readings in the
background and run the live monitor), vibration and network state. The
app does not ask to be exempted from battery optimisation; you can do that
yourself in Android's settings if readings are delayed.

## Where the data is stored

All readings, settings and results are stored only in the app's private
storage on your phone. Other apps cannot read it. Nothing is uploaded to us
or to anyone else, because the app cannot connect to the internet.

## Sharing

We do not share data with anyone. The only way data leaves the app is when
**you** choose **Export** in Settings → Data & backup: the app creates a JSON
file and opens Android's share sheet, and you decide where it goes (for
example a file, an email or a cloud drive of your choice). After that, the
file is handled by the app or service you picked, under its own privacy
policy.

## How long data is kept, and how to delete it

- You choose how long history is kept in Settings → Data & backup → *Keep
  history for* (7, 30, 90, 180 or 365 days, or forever; 90 days by default).
  Older readings are deleted automatically once a day.
- **Delete all history** in Settings → Data & backup removes every recorded
  reading. **Delete history** on an app's page removes that app's records.
- Uninstalling the app, or clearing its storage in Android's settings,
  deletes everything.

## Security

The data never leaves the phone and is kept in the app's private storage,
protected by Android's app sandbox. If you export a file, keep it somewhere
you trust: it contains your recorded history.

## Children

The app is not directed at children under 13 and does not knowingly collect
any information from anyone, including children.

## Changes to this policy

If this policy changes, the new version will be published at this address
with a new effective date. If a future version of the app ever sends data off
the phone, that will be stated here and in the Google Play listing before the
version is released.

## Contact

Questions about this policy: [mezyantbe@gmail.com](mailto:mezyantbe@gmail.com)
