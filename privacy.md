---
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy — Outline Notes

**Last updated:** June 30, 2026

Thank you for using **Outline Notes** ("the App"). This Privacy Policy explains what information the App handles and the choices available to you.

## 1. Who we are

Outline Notes is published by **Xin Sun**, contactable at [**themingledspirit@gmail.com**](mailto:themingledspirit@gmail.com).

## 2. Data we handle

The App is designed to keep your notes and personal data on your own device and (if you enable it) in your own iCloud Drive.

| Data type | Where it lives | Why it's needed |
|---|---|---|
| Outline notes, headers, tags, prayer entries | On your device + your personal iCloud Drive (if enabled) | Core app functionality |
| Photos you scan | Processed **on-device** with Apple Vision (OCR); not uploaded | Convert photos to text |
| PDF files you upload | Text-layer extracted on-device (`pdfjs`); when online, may be processed by our own backend's free `pypdf` text extractor — no AI, no third-party | Convert PDFs to text |
| Rcv API credentials (App ID + Token) | Encrypted on-device in iOS Keychain / Secure Storage | Optional Rcv verse retrieval |

## 3. What we do NOT collect

- No account or login.
- No tracking across other apps or websites.
- No analytics SDKs (no Firebase, Mixpanel, Amplitude, Sentry, Crashlytics, etc.).
- No advertising. No data sale.
- No access to your contacts, location, microphone, calendar, health, or HomeKit.

## 4. Third-party content and services

The App ships with, or may connect to, the following third-party content and services. Each item below is **opt-in** unless noted.

### a. World English Bible (WEB) — bundled offline

When you enable **Settings → Verse Retrieval** with the Rcv sub-toggle OFF, verse text is served from a bundled copy of the **World English Bible**.

The World English Bible is **in the public domain** (<https://worldenglish.bible/>). No license is required to read, quote, or redistribute it. The App stores its text locally as a read-only resource; no external request is made to fetch WEB verses.

### b. Rcv API (`api.lsm.org`) — optional

When you enable **Settings → Verse Retrieval** with the "Rcv" sub-toggle ON and successfully verify your credentials, the App sends the Bible references you type (e.g. `Col. 4:2`) and your personal Rcv API token to `api.lsm.org` over HTTPS. The verse text returned is stored in your local notes.

You must obtain your own Rcv API credentials from <https://api.lsm.org>. We do not own or operate that service. Use is governed by the third-party API provider's terms.

### c. PDF text extraction (free, no AI) — on-device first, our backend as a fallback when online

When you import a PDF, the App first attempts to extract text **on your device** using `pdfjs` (Mozilla's open-source JavaScript PDF parser). If you are online, the App may instead send the PDF to our own backend, which runs the free `pypdf` Python library to extract the embedded text layer and return the result. **No artificial intelligence, no third-party LLM, and no image-recognition service is involved.** PDFs are processed only for text extraction and are not retained on our servers.

The App does **not** perform OCR on the contents of PDFs. If the PDF is a scanned image with no embedded text layer, the App will ask you to use the in-app Camera scanner instead, which runs entirely on-device via Apple Vision.

### d. Apple iCloud — optional

If you enable iCloud sync, your notes are stored in your own iCloud Drive container under your own Apple ID. We do not have access to your iCloud data. Refer to <https://www.apple.com/legal/privacy/>.

## 5. Children's privacy

The App is not directed at children under 13 and we do not knowingly collect personal information from children.

## 6. Data retention & deletion

Because we don't keep your data on our servers, **deleting the App from your device deletes your data**. If iCloud sync is enabled, delete the App's iCloud data from `Settings → Apple ID → iCloud → Manage Storage → Outline Notes`.

You can also export every note at any time from the App's iCloud / Backup screen as a JSON file.

## 7. Security

- All network requests use HTTPS (TLS 1.2+).
- Rcv API credentials live in iOS Secure Storage (Keychain), protected by your device passcode and Secure Enclave.

## 8. Your rights

Subject to your jurisdiction (GDPR, CCPA, PIPEDA, etc.), you may have the right to access, correct, export, or delete personal data we hold about you. Because we don't hold personal data on our servers, these rights are exercised by managing the data on your device. For formal requests email [**themingledspirit@gmail.com**](mailto:themingledspirit@gmail.com).

## 9. Changes to this policy

We will update this page if our practices change. The "Last updated" date above reflects the latest revision.

## 10. Contact

Email: **themingledspirit@gmail.com**
