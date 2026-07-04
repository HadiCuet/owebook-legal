# Owe Book — Privacy Policy

**Effective date:** July 4, 2026

Owe Book is a personal lend-and-borrow tracker — a private notebook for who owes what. This policy explains, in plain English, what data the app handles and the choices you have. The short version: your ledger stays on your device (and, if you turn it on, your own private iCloud), and we never see it.

---

## 1. Who we are

Owe Book is an iOS app developed and operated by **Abdullah Al Hadi** (publishing as Mukashi) ("we", "us"). For the purposes of the EU/UK/EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data handled through the app. For any privacy question, contact **mukashi.dev@gmail.com**.

---

## 2. Data we collect

### Stays only on your device — never sent to us

Everything you record in Owe Book is stored locally on your device using Apple's SwiftData framework. **We have no server that stores your ledger, and we cannot read it.**

- **People** you add — names, phone numbers, and any optional relationship label, whether typed in or picked from your Contacts.
- **Transactions** — amounts, currencies, dates, payment modes, notes, and due dates.
- **Receipt and settlement-proof images** you attach.
- **Groups and bill splits**, and your **settings** (home currency, app-lock and sync preferences).

**iCloud Sync (optional).** If you enable iCloud Sync in Settings, the app mirrors your ledger to the **private** database of your own iCloud account (Apple CloudKit), so it stays in sync across your Apple devices. That data lives in your iCloud, is governed by Apple, and is **not** visible to us. You can turn sync off at any time.

### Sent to Firebase (Google)

We use two Firebase services from Google to improve the app: **Analytics** and **Crashlytics**. Neither uses advertising identifiers, cross-app tracking, or ads.

**Firebase Analytics** collects:

- A per-install device identifier (a Firebase app-instance ID). It cannot identify you across other apps and resets if you reinstall.
- Device model, OS version, app version, language, and country (derived from IP, which Google then discards from the event).
- Anonymous feature-usage events — for example that an entry was created (its type and currency code), that a group had a certain number of members, that the paywall was shown, or that a setting was toggled. Each event carries only categorical values and on/off flags. One user property, `is_pro` (`true`/`false`), records whether Owe Book Pro is unlocked.
- **We never send** the names, phone numbers, amounts, note text, or images in your ledger.

**We do not request App Tracking Transparency** and never read your IDFA. **We never call `setUserID()`** — there is no account and no persistent identity tied to you.

**Firebase Crashlytics** collects data only when the app crashes or reports a handled error: the stack trace, a snapshot of device state (model, OS version, free memory/disk), a per-install Crashlytics identifier, and a small set of non-identifying custom keys we attach to aid triage — currently only the `is_pro` flag. Crash reports are not designed to contain your ledger content.

### Purchases (Owe Book Pro)

Owe Book is free, with an optional one-time in-app purchase (**Owe Book Pro**) handled through Apple's StoreKit. **Apple processes the payment** — your card and billing details are never seen by the app or by us. The app stores whether Pro is unlocked, and analytics records only non-financial purchase events (that a purchase started, completed, or failed, plus the product identifier and price/currency) — never receipts, transaction IDs, or payment methods. **Restore Purchases** asks Apple (not us) which products are tied to your Apple Account.

---

## 3. Permissions the app asks for

- **Contacts** — optional, only when you add a person from your address book. Only the contact you pick (name and phone) is used; we do not read or upload your full contact list.
- **Photos** — optional, only when you attach a receipt or proof image. Only the image you pick is saved with that entry; we do not scan your library.
- **Face ID / passcode** — optional, only when you enable App Lock. The check happens locally via Apple's LocalAuthentication framework; your biometric data never leaves the device and is never seen by the app.
- **Notifications** — optional, only when you schedule a reminder. Used to deliver a local reminder at the time you choose; not used for marketing.

The app does **not** request the camera, microphone, location, calendar, motion, or health data.

---

## 4. How we use this data

- **Local data** powers the app's features — showing your balances, statements, and reminders. It is not used for anything else.
- **Firebase Analytics** tells us, in aggregate, which features are used so we can decide what to improve. We look at counts, not individuals.
- **Firebase Crashlytics** tells us when and why the app crashes so we can fix the bug.

We do **not** sell your personal information, and we do not share it for cross-context behavioural advertising (as those terms are defined under the CCPA/CPRA). We do not build profiles across other apps or share data with advertisers or data brokers.

---

## 5. Who we share data with

The only third party the app sends data to is **Firebase**, operated by Google LLC (and, for EEA/UK/Swiss users, Google Ireland Limited), which processes Analytics and Crashlytics data as our service provider under the [Firebase Data Processing Terms](https://firebase.google.com/terms/data-processing-terms) and [Google Privacy Policy](https://policies.google.com/privacy). Apple processes your in-app purchases and, if you enable it, your iCloud sync, under the [Apple Privacy Policy](https://www.apple.com/legal/privacy/). We may also disclose information where required by valid legal process. No other analytics, advertising, or tracking SDK is bundled in the app.

Google primarily processes Firebase data on servers in the **United States**. For EEA/UK/Swiss users, international transfers rely on the Standard Contractual Clauses incorporated into Google's terms.

---

## 6. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app. Uninstalling removes it.
- **Firebase Analytics** — retained by Google per Firebase's default event retention (up to 14 months).
- **Firebase Crashlytics** — retained by Google for 90 days.

---

## 7. Your rights and choices

- **Edit or delete** any person, transaction, or group directly in the app; turn off iCloud Sync in Settings; or uninstall the app to remove all local data.
- **Turn off analytics system-wide** — iOS **Settings → Privacy & Security → Analytics & Improvements**.
- **Access or erasure** under GDPR (EEA/UK), CCPA/CPRA (California), or similar laws — email **mukashi.dev@gmail.com**. Because analytics data is not tied to a persistent identity, the most reliable erasure is uninstalling the app, which invalidates the per-install identifiers.
- **Lodge a complaint** with your local data-protection authority if you're in the EEA, UK, or Switzerland — though we'd appreciate the chance to help first.

---

## 8. Children's privacy

Owe Book is a general-audience app and is not directed to children under 13 (or the minimum age in your country). We do not knowingly collect personal information from children. If you believe a child has provided us information, email **mukashi.dev@gmail.com** and we will delete it.

---

## 9. Security

- Local data is stored in iOS's app sandbox and encrypted at rest by the device when a passcode is set. You can add an optional Face ID / passcode **App Lock** to the app itself.
- Data synced to iCloud is encrypted in transit and at rest by Apple; data sent to Firebase travels over HTTPS (TLS).
- We operate no server that holds your ledger. No method is perfectly secure, but we keep our data footprint deliberately small and will notify you of a breach as required by law.

---

## 10. Changes & contact

If we change this policy, the new version replaces this page and the "Effective date" above is updated; material changes are noted in the app's release notes. This policy also applies alongside our [Terms of Use](terms.html).

Questions, requests, or complaints: **mukashi.dev@gmail.com**.

---

© 2026 Abdullah Al Hadi (Mukashi). Owe Book.
