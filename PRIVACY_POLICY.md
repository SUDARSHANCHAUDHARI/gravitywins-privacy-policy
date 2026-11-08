# GravityWins — Privacy Policy

**Effective Date:** 2026-03-21
**Last Updated:** 2026-11-08
**Version:** 1.2.0

Published by **Sudarshan Tech Labs** | https://sudarshantechlabs.com | sudarshantechlabs@gmail.com

---

GravityWins is a health and fitness tracking app for Android. Your health and fitness data is stored exclusively on your device. Sudarshan Tech Labs does not operate a backend server and does not collect any personal data. The App does send crash reports to Firebase Crashlytics (Google) when it crashes, as described below.

---

## Data Collection

### Data Stored Locally on Your Device

| Data | Purpose | Storage |
|---|---|---|
| Health and fitness activity data | Core tracking functionality | Room database on your device |
| App settings and preferences | Personalisation | DataStore on your device |

No data is transmitted to Sudarshan Tech Labs or any third-party server.

---

## How We Use Your Data

All data is used solely to provide the in-app tracking experience. No data is shared, analysed externally, or used for advertising.

---

## Data Storage and Security

- **All data is stored locally** in a Room database within the App's private directory
- **No tracking data transmission:** The App does not send your tracking data to any external server. The only outbound traffic is a crash report to Firebase Crashlytics when the App crashes.
- **Android sandbox:** Data is protected by Android's application isolation

## Data Retention

| Data | Retention |
|---|---|
| All local app data | Until you delete it or uninstall the App |

---

## Data Sharing

We do not sell any user data, and your tracking data never leaves your device.

The App does share one thing with a third party:

- **Firebase Crashlytics (Google):** If the App crashes, a crash report is sent to Firebase Crashlytics. It can include the error details, device model, Android version, app version, and an installation identifier. It does not include your tracking data. We use it only to find and fix bugs. Google's handling of this data is covered by the [Firebase Privacy Policy](https://firebase.google.com/support/privacy).

---

## Background Services

GravityWins uses a foreground service (`FOREGROUND_SERVICE_HEALTH`) to track health activity in the background. A persistent notification is displayed while the service is running. You can stop the service at any time by dismissing the notification.

---

## Permissions Explained

The App itself asks for six permissions:

| Permission | Why It Is Needed |
|---|---|
| `ACTIVITY_RECOGNITION` | Detect physical activity and movement for tracking. This is a permission you grant at runtime and can revoke at any time in Android Settings |
| `FOREGROUND_SERVICE` | Run health tracking in the background |
| `FOREGROUND_SERVICE_HEALTH` | Required service type for health data tracking |
| `POST_NOTIFICATIONS` | Display the foreground service notification and activity alerts |
| `RECEIVE_BOOT_COMPLETED` | Restart background tracking after device reboot |
| `VIBRATE` | Haptic feedback for activity alerts |

### Permissions added by Android libraries

The finished app carries four more, declared by the libraries it is built on rather than by the App's own code. They appear in the permission list you see on the Play Store:

| Permission | Comes from | What it does |
|---|---|---|
| `INTERNET` | Firebase Crashlytics | **This is the permission that makes the crash reporting described above possible.** It is the only outbound traffic the App produces |
| `ACCESS_NETWORK_STATE` | Firebase Crashlytics | Lets the library check whether a network exists before attempting to send a crash report |
| `BIND_JOB_SERVICE` | WorkManager | How Android runs scheduled background work |
| `DUMP` | a build-time library | Diagnostic permission. Android grants it only to system apps, so it has no effect here |

`INTERNET` is not declared by the App itself, which is why it does not appear in the table above — but it is in the build you install, and the crash report is what uses it. Nothing else in the App sends anything.

---

## Your Rights and Controls

- **Delete all data:** Uninstall the App or go to Android Settings > Apps > GravityWins > Storage > Clear Data
- **Stop background service:** Dismiss the persistent notification

---

## Children's Privacy

GravityWins is not directed at children under 13. We do not collect any personal information.

---

## Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of significant changes via:

- In-app notification
- Updated policy date on this page

Continued use of GravityWins after changes become effective constitutes your acceptance of the updated policy.

---

## Contact Us

For privacy questions, data access requests, or account deletion:

- **Email:** sudarshantechlabs@gmail.com
- **Developer:** sunny.sudarshan@gmail.com
- **Website:** https://sudarshantechlabs.com
- **Response Time:** Within 48 hours

---

## Play Store Data Safety Summary

| Data type | Collected | Shared | Purpose |
|---|---|---|---|
| Health and fitness data | Local only | No | App functionality |
| Crash logs | Yes | Yes (Google) | Diagnostics |
| Device or other IDs | Yes | Yes (Google) | Diagnostics |

---

---

## Recent Updates (Version 1.2.0 - November 8, 2026)

- **Removed the boilerplate** claiming protection by "Android, the browser, Firebase, Google, GitHub, or other services". Firebase and Google are true for GravityWins, which made the sentence easy to overlook, but the browser and GitHub are not.
- **Kept the Firebase Crashlytics disclosure as written.** It was already accurate — the app does send a crash report, and the policy names what it contains and links Google's own privacy policy. This is the one app in the family that genuinely sends data off the device.
- **Added `INTERNET` to the permissions,** tied explicitly to that crash report. The policy described the crash reporting without ever naming the capability behind it.
- **Added `ACTIVITY_RECOGNITION` to the app-declared permissions** in the app repository's copy, where it had been omitted. It is a runtime permission for physical activity data and the most sensitive one the app requests.
- **Listed the remaining library-merged permissions** — `ACCESS_NETWORK_STATE` from Crashlytics, `BIND_JOB_SERVICE` from WorkManager, and `DUMP` — since the app declares six while the Play Store shows ten.
- **Confirmed and did not disclose webhooks.** The app's own context files describe webhook integration with certificate pinning, but no such code exists: only orphan retry constants remain, with no HTTP client dependency and no URL in the source. A webhook would have sent drop data to a user-configured endpoint and would have required disclosure.

---

## Recent Updates (Version 1.1.0 - May 17, 2026)

- **Aligned policy with the shared privacy-policy structure.**
- **Clarified local health/activity data and Android health-related permissions.**

---

**This privacy policy complies with:**
- Google Play Store requirements
- GDPR (General Data Protection Regulation)
- CCPA (California Consumer Privacy Act)

**Last reviewed:** 2026-11-08

---

This is the published policy, served at https://sudarshanchaudhari.github.io/gravitywins-privacy-policy/ from the `main` branch of this repository. `index.html` carries the same content for the web and must be updated alongside this file. The copy in the [GravityWins app repository](https://github.com/SUDARSHANCHAUDHARI/GravityWins/blob/main/PRIVACY_POLICY.md) is kept identical.
