# Tempo Privacy Policy

Effective date: June 12, 2026

Last updated: June 12, 2026

Tempo ("Tempo", the "App", "we", "us", or "our") is a local-first RSVP reading app provided by Joshua Hoffman. This Privacy Policy explains what information Tempo collects, stores, uses, and shares when you use the App.

Privacy/support contact: hello@temporeader.app

## 1. Summary

Tempo keeps your reading content local by default. We use limited analytics, diagnostics, and purchase services to improve the app and manage purchases.

Important points:

- Tempo does not currently require an account.
- Tempo does not currently provide cloud sync.
- Your imported or pasted reading content is stored locally on your device.
- Tempo uses PostHog for analytics, diagnostics, and session replay when configured. In configured builds, analytics collection is enabled by default unless you turn it off in Settings.
- Tempo uses always-on minimal crash diagnostics when PostHog is configured, even if you turn off analytics and replay.
- Tempo uses RevenueCat to manage in-app purchase offerings, purchase status, and purchase restoration.
- Tempo does not intentionally send your document text, document titles, file names, source file paths, source URLs, or EPUB location data to PostHog.
- Tempo does not receive or store your full payment card information.

## 2. Scope

This Privacy Policy applies to Tempo mobile apps and any support or website surfaces that link to this Privacy Policy.

This Privacy Policy does not apply to third-party apps, websites, app stores, payment providers, operating systems, or share destinations that you choose to use with Tempo. Those services have their own privacy policies and terms.

## 3. Information Stored Locally On Your Device

Tempo stores most app data locally on your device using local app storage, including SQLite/Drift storage and platform preferences.

### Reading Content And Library Data

When you add or import content, Tempo may store:

- Pasted text and pasted Markdown.
- Imported TXT file text.
- Extracted PDF text.
- Extracted EPUB text.
- Extracted images from supported PDF and EPUB imports.
- Archived copies of imported source files when the import flow stores a local source archive.
- Document titles you enter, rename, or that Tempo derives from the content or file name.
- Source type, such as pasted text, TXT, Markdown, PDF, or EPUB.
- Source metadata, such as source URI, original file name, MIME type, file size, importer name, and importer version.
- Parsed document structure, such as blocks, headings, lists, quotes, tables, page or chapter markers, sentences, tokens, token styles, source ranges, page numbers, chapter indexes, EPUB CFI values, and image metadata.
- Plain text derived from imported or pasted content.
- Raw content used to support editing and reparsing.

### Reading Progress, Usage, And Stats

Tempo may store local reading activity, including:

- Current token or reading position for a document.
- Words displayed during playback.
- Reading speed in words per minute.
- Document completion status.
- Local reading sessions, including start time, end time, and active duration.
- Daily streak progress.
- Trial usage ranges and daily trial usage ranges.
- Total words read, words read today, reading days, completed texts, streak counts, weekly activity, monthly activity, and active reading time.

Tempo currently counts trial and streak progress only for words displayed during RSVP playback, not merely for content you import or view while paused.

### Preferences And App Settings

Tempo may store settings and preferences, including:

- Theme mode and theme preset.
- Font choices.
- Reader text size and RSVP word size.
- RSVP focal column position.
- Default WPM.
- Timing comfort preset and advanced timing values.
- Whether images should open automatically while reading.
- Onboarding and tutorial completion state.
- Post-tutorial coachmark completion state.
- Analytics collection preference.
- Paywall experiment variant.
- Local entitlement state used to remember whether unlimited reading is enabled.

## 4. Information Sent To Tempo's Service Providers

Tempo uses limited third-party services for analytics, diagnostics, and purchases.

### PostHog Analytics And Session Replay

Tempo uses PostHog to understand whether onboarding, imports, reader controls, trial limits, and paywall flows are working as intended.

When PostHog is configured and analytics collection is enabled, Tempo may send events to PostHog Cloud, currently using PostHog's U.S. ingestion endpoint unless a build is configured otherwise. Tempo may send events such as:

- App and screen events, including settings, stats, import sheet, reader, tutorial reader, and paywall screens.
- Import flow events, including source selection, import start, import success, and import failure.
- Import metadata, such as source type, error type, and bucketed word count.
- Onboarding events, including tutorial opened, playback started, tutorial completed, and coachmarks completed.
- Reader events, including document opened, playback started, playback paused, and reader session completed.
- Reader metadata, such as source type, bucketed word count, bucketed WPM, and whether the document is the tutorial.
- Trial events, including trial milestones, daily limit reached, and lifetime limit reached.
- Trial metadata, such as entitlement status, whether unlimited access is enabled, trial percentage, and bucketed daily and total word counts.
- Paywall events, including paywall shown, dismissed, purchase tapped, restore tapped, and purchase result.
- Paywall metadata, such as trigger, variant, offer kind, result status, whether a price is present, and whether a package identifier is present.
- Technical and system properties automatically added by PostHog or the platform SDK, such as device type, operating system, app/session identifiers, app lifecycle information, approximate network-derived information, and diagnostic metadata.
- Tempo's anonymous app instance ID, which is the same value shown as the Support ID.

Tempo's PostHog configuration includes safeguards:

- Analytics collection is enabled by default in builds where PostHog is configured, unless you turn it off.
- Analytics collection can be turned off in Settings when PostHog is available in the build.
- Turning analytics off disables future product analytics events and stops session recording, but minimal crash diagnostics remain on.
- Session replay is configured to mask all text and images.
- Reader and import screens are wrapped in an explicit replay mask.
- PostHog surveys are disabled.
- A sanitizer removes event properties whose keys indicate sensitive content or identity, including content, document text, email, EPUB CFI, file names, paths, raw values, source URI, text, title, and URI.

Tempo does not intentionally send your reading content, document titles, file names, source file paths, source URLs, or EPUB CFI values to PostHog. However, analytics, session replay, and crash diagnostics tools can still process interaction metadata, screen structure, device data, session identifiers, stack traces, app version, build number, anonymous app instance ID, anonymous Support ID, and other technical data. If you do not want Tempo to send product analytics or replay data, turn off "Analytics and replay" in Settings. Crash diagnostics remain on to help keep the App stable.

When session replay is enabled, a crash report may be associated with the same masked session recording so we can understand the steps that led to a crash. If analytics and replay are turned off, crash diagnostics may still be sent, but without replay context.

PostHog may queue events locally while the device is offline and send them later when the device is online. Turning analytics off prevents future collection, but it does not automatically delete events that were already sent to PostHog.

PostHog privacy information: https://posthog.com/privacy

### RevenueCat Purchases

Tempo uses RevenueCat to load purchase offerings, start purchases, restore purchases, and check whether the `unlimited_reading` entitlement is active.

Tempo currently configures RevenueCat for iOS builds when a RevenueCat Apple API key is available. Future builds may support additional platforms.

RevenueCat and the applicable app store may process:

- Tempo's anonymous app instance ID as the RevenueCat App User ID, which is the same value shown as the Support ID.
- CustomerInfo and entitlement status.
- Purchase offering and package information.
- Purchase and restore results.
- Store receipt data, such as Apple receipt files or Google purchase tokens, depending on platform.
- End-user technical information, such as device type, operating system, and last seen time.

Tempo does not currently provide RevenueCat with a Tempo account email because Tempo does not currently have accounts. Tempo does not receive or store your full credit card number. Payments, taxes, refund handling, and store account authentication are handled by the applicable app store and related payment systems.

RevenueCat privacy information: https://www.revenuecat.com/privacy

### App Stores And Payment Providers

If you purchase or restore Tempo through Apple App Store, Google Play, or another app marketplace, that marketplace may process your store account, payment method, tax information, transaction history, receipts, refund requests, device information, and fraud-prevention data under its own policies.

Apple privacy information: https://www.apple.com/legal/privacy

Google privacy information: https://policies.google.com/privacy

### File Picker, Operating System Services, And Share Destinations

Tempo uses platform file picker and sharing features. When you choose a file, the operating system may provide Tempo access to that selected file. When you choose to share a streak, completion, text, or screenshot, Tempo passes the share payload to the operating system share sheet and to the destination app or service you choose.

Those destinations may collect, store, or share what you send according to their own policies. Do not share content through a destination unless you are comfortable with that destination receiving it.

## 5. How We Use Information

Tempo uses information to:

- Provide the reader, library, import, parsing, review, progress, stats, streak, and settings features.
- Store and reopen documents locally.
- Resume reading where you left off.
- Count trial usage and daily streak progress.
- Enforce trial limits and unlock unlimited local reading after purchase.
- Load purchase offers, complete purchases, restore purchases, and refresh entitlement status.
- Improve app quality, onboarding, imports, reader controls, and paywall flows.
- Detect import failures, crashes, performance issues, and product issues.
- Respond to support requests.
- Comply with legal, tax, fraud-prevention, security, and app-store obligations.

## 6. How Information Is Shared

- With PostHog for analytics and session replay when enabled, and for minimal crash diagnostics when PostHog is configured.
- With RevenueCat for purchase offering, entitlement, purchase, and restore handling.
- With Apple, Google, or another marketplace when you install, purchase, restore, request a refund, or manage purchases through that marketplace.
- With operating system services and share destinations when you choose to import or share content.
- With service providers that help us operate, support, secure, analyze, or improve Tempo.
- If required by law, legal process, regulation, court order, or government request.
- To protect rights, safety, security, users, or the public.
- In connection with a merger, acquisition, financing, reorganization, sale of assets, or similar business transaction.
- With your consent or at your direction.

We do not sell your reading content.

## 7. Data Retention

Local app data remains on your device until you delete it, uninstall the App, clear app data, or your operating system removes it.

When you delete a document in Tempo, the App removes it from your local library, clears the stored document content and parsed reader data, and attempts to delete archived source files and extracted image files associated with that document. Local reading history may remain for stats until you use the delete reading history option in Settings.

Some data may remain outside Tempo's local storage:

- Device backups may retain app data depending on your operating system and backup settings.
- Analytics data already sent to PostHog may remain according to PostHog project retention settings.
- Purchase and entitlement data may remain with RevenueCat and app stores according to their retention policies and legal obligations.
- Content you share to another app or service is controlled by that destination after sharing.
- Support messages you send to us may be retained as needed to respond, keep records, and comply with legal obligations.

## 8. Your Choices And Controls

You can:

- Delete individual documents from the local library.
- Edit or rename supported local text entries.
- Turn off analytics and replay in Settings when analytics is configured.
- Use the app without creating a Tempo account because accounts are not currently required.
- Request a purchase restore through the App.
- Delete Tempo from your device to remove local app data, subject to operating-system backups and marketplace records.
- Contact us to request access, correction, deletion, or other rights for data we control.

Because Tempo currently has no account system, we may need information from you to locate third-party analytics or purchase records, such as a RevenueCat App User ID, app-store transaction information, support email address, or enough context to identify the relevant record.

## 9. Regional Privacy Rights

Depending on where you live, you may have rights to request access, correction, deletion, portability, restriction, objection, withdrawal of consent, or appeal of certain privacy decisions.

If you are in the European Economic Area, United Kingdom, or Switzerland, our legal bases may include:

- Performance of a contract, to provide Tempo and paid features.
- Legitimate interests, to improve, secure, debug, and support the App.
- Consent or user choice, where required for analytics, replay, marketing, or similar processing.
- Legal obligations, to comply with tax, accounting, app-store, fraud-prevention, and legal requirements.

If you are in California or another U.S. state with privacy rights, you may have rights to know, access, correct, delete, or opt out of certain uses of personal information. Tempo does not intentionally sell personal information or share it for cross-context behavioral advertising.

To exercise rights, contact hello@temporeader.app.

## 10. Children

Tempo is not directed to children under 13, or the equivalent minimum age in your jurisdiction. We do not knowingly collect personal information from children below that age. If you believe a child has provided personal information to us, contact hello@temporeader.app.

## 11. Security

Tempo uses platform app storage and limits third-party analytics properties to reduce exposure of reading content. No method of storage or transmission is completely secure. You are responsible for protecting access to your device, backups, store accounts, and any shared files or screenshots.

## 12. International Transfers

Tempo's service providers may process information in the United States and other countries. If you use Tempo outside the United States, your information may be processed in jurisdictions that may have different data protection laws than your location.

## 13. Future Features

Tempo may later add features such as website import, optional sync, backup, accounts, email support, or cloud services. If those features materially change what information is collected, stored, used, or shared, we will update this Privacy Policy before those features are released.

## 14. Changes To This Privacy Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last updated" date above. If changes are material, we will provide notice as required by law or platform rules.

## 15. Contact

For privacy questions or requests, contact Joshua Hoffman.

Privacy/support contact: hello@temporeader.app
