# GravityWins Privacy Policy

This repository contains the public privacy policy for GravityWins.

- Privacy policy: [PRIVACY_POLICY.md](PRIVACY_POLICY.md)
- Web version: https://sudarshanchaudhari.github.io/gravitywins-privacy-policy/
- Contact: sunny.sudarshan@gmail.com

## What not to lose from this policy

GravityWins is the one app in this family that genuinely sends data off the device: **Firebase Crashlytics** receives a crash report when the app crashes, and that is what the merged `INTERNET` permission is for. The policy names the recipient, says what the report contains, and links Google's own privacy policy.

It also declares `ACTIVITY_RECOGNITION`, a runtime permission for physical activity data.

Any future edit must keep both disclosures.

Note that `webhooks` are **not** a feature of this app, despite the app repo's `CLAUDE.md` and `AGENTS.md` describing them. Only orphan retry constants remain in `TimeConstants.kt`, there is no HTTP client dependency, and no URL in the Kotlin source. Do not add a webhook disclosure unless the code actually gains one.

## Editing

`PRIVACY_POLICY.md` is the source of truth. `index.html` carries the same content for GitHub Pages and must be updated in the same commit — Pages serves `main` at the repository root with no build step, so a change to the Markdown alone does not reach the published page.

The copy in the [GravityWins app repository](https://github.com/SUDARSHANCHAUDHARI/GravityWins/blob/main/PRIVACY_POLICY.md) is kept identical to this one.

This README no longer duplicates the policy text. It used to, which left three copies of the same document drifting apart.
