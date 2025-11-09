# GravityWins Privacy Policy

_Last updated: November 9, 2025_

GravityWins (“we,” “our,” or “us”) is a personal drop-tracking app. This Privacy Policy explains what information the app collects, how it is used, and the choices you have. By installing or using GravityWins you agree to the practices described below.

## Information We Collect

GravityWins is designed to work primarily offline. The app stores the following information on your device:

- **Drop activity and statistics:** Timestamps of recorded drops, daily and lifetime totals, streaks, and last-drop time.
- **Drop context:** Optional notes and tags you add to individual drops.
- **User preferences:** Notification settings, quiet-hour schedule, focus-mode timers, home layout choice, telemetry toggle, daily goals, milestone unlocks, webhook configuration, and export/reminder preferences.
- **Weekly digest summaries:** Aggregated counts (e.g., drops per week, busiest hour or weekday) generated for the in-app digest.
- **Telemetry events (optional):** Basic app-usage events (for example “drop detected,” “history exported,” or “contact request started”) are buffered in memory only when telemetry is enabled. They are not transmitted anywhere in the current build.

The app **does not** collect precise or approximate location, contact lists, photos, audio, or persistent device identifiers. Accelerometer readings are processed on-device to detect drops; raw sensor data is not stored.

### Information You Choose to Share

- **Contact form:** If you fill out the “Need help or want to contribute?” form, your name, reply email, subject, and message are placed into an email draft addressed to the developer (`sunny.sudarshan@gmail.com`). The app does not keep a copy; sending the message is handled entirely by your chosen email provider.
- **Data exports:** When you export history as CSV or JSON, the files are created in the app’s private cache and shared through Android’s system share sheet. The data leaves your device only if you choose a destination (e.g., email, cloud storage).
- **Webhooks:** If you enable webhooks, drop summaries (counts, humor line, timestamps, and—if you opt in—device model/manufacturer/Android version) are sent to the HTTPS endpoint you configure. We do not run or control that endpoint.

## How We Use Information

All collected information is used strictly to provide app functionality:

- Maintain drop counts, streaks, and history.
- Drive focus-mode, notifications, widgets, and reminders.
- Populate weekly digests and diagnostic timelines.
- Send optional webhooks and exports that you initiate.
- Improve the experience based on optional telemetry events (currently only saved in memory).

We do not run ads and do not sell, rent, or monetize your data.

## Storage and Retention

- Drop history, preferences, and digests are stored locally using Android DataStore and Room database.
- Exported CSV/JSON files live in a cache directory until you share them or the app clears old files (the app retains up to five recent exports).
- Telemetry events are held in memory only and cleared when the app restarts.
- Webhook dispatch logs are in-memory and capped to the five most recent attempts.

If you uninstall GravityWins, all locally stored data is removed from your device.

## Sharing and Transfers

We do not send data to our own servers or third-party analytics services. Data leaves the device only when you:

- Send an email via the contact form.
- Share a CSV/JSON export through another app or service.
- Configure a webhook endpoint.

Because those actions are user-directed, any further processing is governed by the recipient service’s policies.

## Your Choices and Controls

- **Telemetry:** Toggle analytics events on or off in Settings → Diagnostics. When off, no events are recorded.
- **Drop history:** Edit notes/tags, clear individual entries, or clear all history in Settings.
- **Exports:** Delete exported files through the target app/service or clear the app’s cache.
- **Webhooks:** Enable/disable the feature at any time, update the destination URL, and choose whether device info is included.
- **Quiet hours and notifications:** Customize in Settings or disable entirely.
- **Data removal:** Uninstalling the app deletes all information stored by GravityWins.

## Security

Data remains on your device unless you choose to share it. For webhooks the app uses HTTPS when supported by the destination. Because exports and emails are user-directed, ensure you trust the recipients you select. Data stored locally (drop history, preferences) is not encrypted on your device. Standard Android security protections apply.

## Children’s Privacy

GravityWins is intended for a general audience and is not directed at children under 13. If you are a parent or guardian and believe your child has provided personal information, contact us to request deletion.

## Changes to This Policy

We may update this Privacy Policy to reflect new features or legal requirements. Significant changes will be noted in the app release notes or within the documentation. The “Last updated” date at the top will change when revisions occur.

## Contact Us

If you have questions about this Privacy Policy or wish to request data deletion, contact:

- **Email:** sunny.sudarshan@gmail.com  
- **App:** Open GravityWins → About → “Need help or want to contribute?”

We will respond as quickly as possible.


