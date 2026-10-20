# Owe Book — Privacy Policy

**Effective date:** October 20, 2026

Owe Book is a personal lend-and-borrow tracker for iPhone, iPad and Mac — a private notebook for who owes what. This policy explains, in plain English, what data the app handles and the choices you have. The short version: your ledger stays on your devices (and, if you use iCloud Sync, your own private iCloud), groups you share reach only the people in them, through Apple's iCloud, and we never see any of it.

---

## 1. Who we are

Owe Book is an app for iPhone, iPad and Mac developed and operated by **Abdullah Al Hadi** (publishing as Mukashi) ("we", "us"). For the purposes of the EU/UK/EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data handled through the app. For any privacy question, contact **mukashi.dev@gmail.com**.

---

## 2. Data we collect

### Stays on your devices — never sent to us

Everything you record in Owe Book is stored locally on your device using Apple's SwiftData framework. **We have no server that stores your ledger, and we cannot read it.**

- **People** you add — names, phone numbers, and any optional relationship label, whether typed in or picked from your Contacts.
- **Entries** — amounts, currencies, dates, payment modes, notes, due dates, and repeat schedules.
- **Receipt and settlement-proof images** you attach.
- **Groups and bill splits**, and your **settings** (home currency, app-lock, sync and reminder preferences).

**Backups.** The app keeps a recovery copy of your ledger on the device, so it can be put back if something goes wrong. **Export Backup** saves a file of your ledger wherever you choose; from then on, that file is yours to keep or delete.

**iCloud Sync (Owe Book Pro).** When iCloud Sync is on in Settings, the app mirrors your ledger to the **private** database of your own iCloud account (Apple CloudKit), so it stays the same on your iPhone, iPad and Mac. That data lives in your iCloud, is governed by Apple, and is **not** visible to us. You can turn sync off at any time. iCloud Sync is part of Owe Book Pro and stays free for anyone who used Owe Book before version 1.4. If Pro ends, sync stops and your ledger stays on the device.

### Shared groups — stored in iCloud, shared through Apple

A group can be shared by its **owner** (who needs Owe Book Pro) with the people they invite, using Apple's iCloud (CloudKit) sharing. Invitations go out through Apple's sharing sheet — Messages, Mail or a link — and anyone invited joins free. A shared group is stored in the owner's iCloud and shared through Apple with everyone in it, and each of them can read and change it. A shared group holds:

- the group's name, currency and icon;
- the members' names, as typed by anyone in the group;
- expenses (title, amount, date, note, who paid and how it's split) and payments;
- receipt photos attached to its expenses;
- for each member someone has marked as "this is me", an anonymous iCloud user identifier linking that member to their Apple account.

Apple's sharing screens show participants' names or contact details according to Apple's rules. Shared groups always sync through iCloud — in a separate iCloud container from your personal ledger — whether or not iCloud Sync is on. The owner can stop sharing the group or delete it for everyone; anyone else can leave, which removes the group from their devices. **We never see any of it.**

### Handled on your device

- **Receipt reading (Owe Book Pro)** — reading the amount from a receipt photo happens on your device with Apple's text recognition. The photo isn't sent anywhere for it.
- **Siri & Shortcuts (Owe Book Pro)** — when you add an entry with Siri or Shortcuts, Apple processes the voice request under Apple's terms. Owe Book only receives the entry details, and saves them on your device.
- **Widgets** — show your balances and due entries on the Home Screen, Lock Screen and StandBy, using data already on your device. They're hidden while App Lock is on.

### Sent to Firebase (Google)

We use two Firebase services from Google to improve the app: **Analytics** and **Crashlytics**. Neither uses advertising identifiers, cross-app tracking, or ads.

**Firebase Analytics** collects:

- A per-install device identifier (a Firebase app-instance ID). It cannot identify you across other apps and resets if you reinstall.
- Device model, OS version, app version, language, and country (derived from IP, which Google then discards from the event).
- Anonymous feature-usage events — for example that an entry was created (its type and currency code), that a group had a certain number of members, that a group was shared, joined or left, which paywall was shown, or that a setting was toggled. Each event carries only categorical values, counts and on/off flags. One user property, `is_pro` (`true`/`false`), records whether Owe Book Pro is unlocked.
- **We never send** the names, phone numbers, amounts, note text, or images in your ledger or your groups.

**We do not request App Tracking Transparency** and never read your IDFA. **We never call `setUserID()`** — there is no account and no persistent identity tied to you.

**Firebase Crashlytics** collects data only when the app crashes or reports a handled error: the stack trace, a snapshot of device state (model, OS version, free memory/disk), a per-install Crashlytics identifier, and a small set of non-identifying custom keys we attach to aid triage — currently only the `is_pro` flag. Crash reports are not designed to contain your ledger content.

### Purchases (Owe Book Pro)

Owe Book is free, with optional paid plans (**Owe Book Pro** — a monthly or yearly subscription, or a one-time purchase; new subscribers to the yearly plan get a 7-day free trial) handled through Apple's StoreKit. **Apple processes the payment** — your card and billing details are never seen by the app or by us. The app stores whether Pro is unlocked, and analytics records only purchase events — that a free trial started, or that a purchase started, completed, or failed, with the product identifier (plus the price and currency, for paid purchases only) — never receipts, transaction IDs, or payment methods. **Restore Purchases** asks Apple (not us) which products are tied to your Apple Account.

---

## 3. Permissions the app asks for

- **Contacts** — optional, only when you add a person from your address book. Only the contact you pick (name and phone) is used; we do not read or upload your full contact list.
- **Photos** — optional, only when you attach a receipt or proof image. Only the image you pick is saved with that entry; we do not scan your library.
- **Face ID / Touch ID** — optional, only when you turn on App Lock (Owe Book Pro). The check happens locally via Apple's LocalAuthentication framework, with your device passcode (or Mac login password) as the fallback; your biometric data never leaves the device and is never seen by the app.
- **Notifications** — optional, and only for local reminders: due-date reminders you set, and a reminder two days before a free trial ends (if you start a trial and haven't allowed notifications yet, the app asks then). Never used for marketing.

The app does **not** request the camera, microphone, location, calendar, motion, or health data.

---

## 4. How we use this data

- **Local data** powers the app's features — showing your balances, statements, Insights, widgets, and reminders. It is not used for anything else.
- **Shared group data** is used only to show the group, and keep it in sync, for the people in it.
- **Firebase Analytics** tells us, in aggregate, which features are used so we can decide what to improve. We look at counts, not individuals.
- **Firebase Crashlytics** tells us when and why the app crashes so we can fix the bug.

We do **not** sell your personal information, and we do not share it for cross-context behavioural advertising (as those terms are defined under the CCPA/CPRA). We do not build profiles across other apps or share data with advertisers or data brokers.

---

## 5. Who we share data with

Apart from Apple, the only third party the app sends data to is **Firebase**, operated by Google LLC (and, for EEA/UK/Swiss users, Google Ireland Limited), which processes Analytics and Crashlytics data as our service provider under the [Firebase Data Processing Terms](https://firebase.google.com/terms/data-processing-terms) and [Google Privacy Policy](https://policies.google.com/privacy). Apple processes your in-app purchases, your iCloud sync if you use it, shared groups, and Siri requests, under the [Apple Privacy Policy](https://www.apple.com/legal/privacy/). Anything added to a shared group is shared, through Apple and not us, with everyone in that group. We may also disclose information where required by valid legal process. No other analytics, advertising, or tracking SDK is bundled in the app.

Google primarily processes Firebase data on servers in the **United States**. For EEA/UK/Swiss users, international transfers rely on the Standard Contractual Clauses incorporated into Google's terms.

---

## 6. How long we keep it

- **Local data**, including the on-device recovery copy — kept on your device until you delete it or uninstall the app. Uninstalling removes it. A backup file you export stays wherever you saved it until you delete it.
- **iCloud Sync data** — kept in your private iCloud, under Apple's control, until you delete it.
- **Shared groups** — kept in the owner's iCloud until the owner deletes the group. Leaving a group removes it from your devices; when the owner stops sharing or deletes it, the people in it lose access.
- **Firebase Analytics** — retained by Google per Firebase's default event retention (up to 14 months).
- **Firebase Crashlytics** — retained by Google for 90 days.

---

## 7. Your rights and choices

- **Edit or delete** any person, entry, or group directly in the app; turn off iCloud Sync in Settings; leave a shared group (or, as its owner, stop sharing or delete it); or uninstall the app to remove all local data.
- **Analytics** — the app has no switch of its own for Firebase Analytics, and it doesn't follow the system's Analytics & Improvements setting. Because the data isn't tied to an account or to you, uninstalling the app resets its identifiers; you can also ask us to delete what's linked to your install (see below).
- **Access or erasure** under GDPR (EEA/UK), CCPA/CPRA (California), or similar laws — email **mukashi.dev@gmail.com**. Because analytics data is not tied to a persistent identity, the most reliable erasure is uninstalling the app, which invalidates the per-install identifiers.
- **Lodge a complaint** with your local data-protection authority if you're in the EEA, UK, or Switzerland — though we'd appreciate the chance to help first.

---

## 8. Children's privacy

Owe Book is a general-audience app and is not directed to children under 13 (or the minimum age in your country). We do not knowingly collect personal information from children. If you believe a child has provided us information, email **mukashi.dev@gmail.com** and we will delete it.

---

## 9. Security

- Local data is stored in the app's sandbox and encrypted at rest by your device when a passcode (or, on a Mac, FileVault) is on. You can add an optional Face ID / Touch ID **App Lock** (Owe Book Pro) to the app itself, which also hides your widgets.
- Data in iCloud — your synced ledger and shared groups — is encrypted in transit and at rest by Apple; data sent to Firebase travels over HTTPS (TLS).
- We operate no server that holds your ledger or your groups. No method is perfectly secure, but we keep our data footprint deliberately small and will notify you of a breach as required by law.

---

## 10. Changes & contact

If we change this policy, the new version replaces this page and the "Effective date" above is updated; material changes are noted in the app's release notes. This policy also applies alongside our [Terms of Use](terms.html).

Questions, requests, or complaints: **mukashi.dev@gmail.com**.

---

© 2026 Abdullah Al Hadi (Mukashi). Owe Book.
