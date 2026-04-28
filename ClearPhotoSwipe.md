# Privacy Policy

**App:** ClearPhoto Swipe
**Bundle ID:** `com.angel.ClearPhoto`
**Apple App ID:** `6764064235`
**Platform:** iOS 18 and later (iPhone, iPad)
**Last updated:** April 28, 2026

This Privacy Policy describes what data is processed by the **ClearPhoto Swipe** mobile application (the "App") and how your privacy is protected. By using the App, you agree to the practices described below.

---

## 1. Who we are

The App is developed by an individual developer holding Apple Developer Team ID `45MPCAL9UB`.

For any privacy-related questions or requests, contact:
[vrnrelax@gmail.com](mailto:vrnrelax@gmail.com)

---

## 2. Summary (TL;DR)

- The App runs **entirely on your device**.
- Photos and their analysis **never leave your device** and are never uploaded to the developer's servers or any third party.
- The App does **not** use third-party analytics, advertising, attribution, crash-reporting, or tracking SDKs.
- The App does **not** track you across other apps and websites (no App Tracking Transparency prompt).
- The only data linked to you is your **subscription status**, handled by Apple via StoreKit.

---

## 3. Data we process

### 3.1 Photos and videos from your library

The App requests access to the iOS Photos library to:

- display your photos and videos,
- group them by month,
- detect similar shots and bursts,
- mark photos as Favorite in the system Photos library,
- move photos you confirm for deletion to the system "Recently Deleted" album.

All of the above happens **locally on the device**. Your photos and videos are never copied off the device by the App and are never transmitted to the developer or any third party.

The App supports the iOS **Limited Photos Library** mode (`PHAuthorizationStatus.limited`). If you grant access only to selected photos, the App will work only with that selection.

### 3.2 Similar-photo analysis (on-device)

To find similar shots and bursts, the App uses Apple's **Vision Framework** (`VNGenerateImageFeaturePrintRequest`). Image feature prints are computed and compared **exclusively on the device**.

Feature prints are **not persisted**: they are generated in memory, used for comparison, and discarded. Nothing derived from your images is sent off the device or stored after the analysis session ends.

### 3.3 User progress (local storage)

The App stores the following on the device using `UserDefaults` to remember your progress between sessions:

- identifier of the currently selected month,
- identifiers of photos you have already reviewed,
- identifiers of photos placed in the in-app trash,
- the count of resolved similar-photo groups (used for the free trial limit),
- a cached flag indicating whether your subscription is currently active.

This data **never leaves your device** and is removed when you uninstall the App.

### 3.4 Purchases (subscription status)

When you purchase the subscription, the App receives from Apple's **StoreKit 2** only the information required to unlock paid features (active / inactive entitlement, transaction verification result). Payment details, your Apple ID and billing information are handled by Apple and are **not** accessible to the App or the developer.

---

## 4. What we do NOT collect

The App does not collect, store, or transmit:

- names, emails, phone numbers, postal addresses, or any other contact data;
- precise or approximate location;
- device identifiers, advertising identifiers (IDFA), or user identifiers created by the App;
- usage analytics, screen views, taps, sessions, or behavioral telemetry;
- crash reports or diagnostics (beyond what Apple itself collects at the OS level when you opt in to share with developers via iOS Settings);
- contacts, calendar, microphone, camera, or health data;
- browsing or search history;
- the contents of your photos or any data derived from them.

The App does not share photos or any data derived from them with third parties.

The App does **not** track you across other apps or websites (Apple's App Tracking Transparency prompt is not requested and is not required).

---

## 5. System permissions

The App requests the following iOS permissions:

| Permission | Type | Why it is needed |
|---|---|---|
| **Photos** | `PHPhotoLibrary.requestAuthorization(for: .readWrite)` | **Read:** load photos and metadata for display, monthly grouping, and on-device similarity analysis. **Write:** toggle the system "Favorite" flag and move photos to "Recently Deleted" upon explicit user confirmation. |

The App does **not** request: Location, Camera, Microphone, Contacts, Bluetooth, Local Network, Calendars, Reminders, Health, Motion, or App Tracking Transparency.

You can review or revoke the Photos permission at any time in:
**iOS Settings → Privacy & Security → Photos → ClearPhoto Swipe**

---

## 6. Subscriptions and payments

The paid subscription (auto-renewable, product ID `com.angel.ClearPhoto.sub`) is processed through Apple's in-app purchase system (**StoreKit 2**). All payments, renewals, refunds, and subscription management are handled by **Apple**, not by the App.

- Subscription verification is performed locally via Apple's signed `JWS` transactions (`VerificationResult`); no developer-operated server is involved.
- You can manage or cancel the subscription at any time in **Settings → [your name] → Subscriptions** on your iOS device.
- You can restore previous purchases at any time using the "Restore Purchases" button on the paywall screen.

The free, non-subscription functionality of the App (swipe review, monthly browsing, trash) remains available without payment.

---

## 7. Local data storage and deletion

| Data | Storage | Removed when |
|---|---|---|
| User progress (reviewed/trash IDs, selected month, counters, subscription flag) | `UserDefaults` (app container) | you uninstall the App |
| Image thumbnails | `NSCache` in RAM | the App is closed or the system reclaims memory |
| System image cache | Managed by `PHCachingImageManager` | managed by iOS |

Uninstalling the App removes all data stored by the App on your device. The App does not retain any backups outside your device.

---

## 8. Network activity

The App does **not** make direct network requests to its own or any third-party servers in normal operation.

Indirect network activity may occur through Apple system APIs that the App relies on:

- **StoreKit** — Apple may contact the App Store to load product information, perform purchases, and validate entitlements.
- **PhotoKit** — if you use **iCloud Photos**, iOS may transparently download originals from iCloud when the App requests them. This is iOS behavior governed by your iCloud settings.
- **External links** — opening Privacy Policy or Terms of Use links launches the system browser.

The App uses no custom backend, no analytics endpoint, no advertising network, and no third-party SDKs.

---

## 9. Third-party services and SDKs

**The App contains no third-party SDKs.** Only Apple system frameworks are used: SwiftUI, PhotoKit, Vision, StoreKit 2, Combine, UIKit (for tab bar appearance), Foundation.

No: Firebase, Crashlytics, Sentry, Mixpanel, Amplitude, AppsFlyer, Adjust, Branch, Google Analytics, Meta/Facebook SDK, TikTok SDK, or any other third-party analytics, attribution, advertising, or crash-reporting library.

---

## 10. Children's privacy

The App is rated **4+** but is **not directed to children under 13** (or the equivalent minimum age in your jurisdiction). The App does not knowingly collect personal information from children. Since the App does not collect personal data from any user, no special children's data is collected either.

---

## 11. Your rights (GDPR / CCPA / similar)

The App does **not collect personal data** from you on the developer side. There is therefore no personal-data record on our side to access, correct, export, restrict, or delete.

- All on-device data can be removed by uninstalling the App.
- Subscription and payment data is held by Apple under Apple's [Privacy Policy](https://www.apple.com/legal/privacy/).
- For any privacy-related question, contact us at [vrnrelax@gmail.com](mailto:vrnrelax@gmail.com). You also have the right to lodge a complaint with your local data protection authority.

---

## 12. Changes to this Policy

We may update this Privacy Policy from time to time. The current version is always available at the URL provided on the App Store listing and inside the App. The "Last updated" date at the top reflects the date of the latest revision. Material changes will be reflected by updating that date.

---

## 13. Contact

For privacy-related inquiries:
[vrnrelax@gmail.com](mailto:vrnrelax@gmail.com)
