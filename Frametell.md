# Privacy Policy

**App:** Frametell
**Bundle ID:** `kd.vlad.Frametell`
**Apple Developer Team ID:** `R7VC35BR98`
**Platform:** iOS 26 and later (iPhone, iPad)
**Last updated:** May 4, 2026

This Privacy Policy describes what data is processed by the **Frametell** mobile application (the "App") and how your privacy is protected. By using the App, you agree to the practices described below.

---

## 1. Who we are

The App is developed by an individual developer (Individual Entrepreneur Vladislav Kolupaev) holding Apple Developer Team ID `R7VC35BR98`.

For any privacy-related questions or requests, contact:
[vrnrelax@gmail.com](mailto:vrnrelax@gmail.com)

---

## 2. Summary (TL;DR)

- The App runs **entirely on your device**.
- Photos and captions **never leave your device** and are never uploaded to the developer's servers or any third party.
- The App does **not** use third-party analytics, advertising, attribution, crash-reporting, or tracking SDKs.
- The App does **not** track you across other apps and websites (no App Tracking Transparency prompt).
- The only data linked to you is your **Frametell Pro purchase status**, handled by Apple via StoreKit.

---

## 3. Data we process

### 3.1 Photos from your library

The App requests access to the iOS Photos library to:

- import photos you select for a carousel,
- save rendered carousel frames into a dedicated **"Frametell"** album in your library.

All processing happens **locally on the device**. Your photos are never copied off the device by the App and are never transmitted to the developer or any third party.

### 3.2 Captions and project state

Captions you type, the chosen format (square / story), and the chosen font are stored as a **local JSON manifest** plus image files inside the App's sandbox (Documents directory). They never leave your device. They are removed when you delete a project from History or uninstall the App.

### 3.3 Onboarding flag (UserDefaults)

The App stores a single boolean (`hasOnboarded`) in `UserDefaults` to remember that you have already seen the onboarding screen. This flag stays on the device, is removed on uninstall, and is declared in the App's `PrivacyInfo.xcprivacy` manifest under reason **CA92.1** (User defaults accessible only to the app itself).

### 3.4 Purchases (Frametell Pro)

When you purchase **Frametell Pro** (`com.frametell.pro`, non-consumable, one-time purchase), the App receives from Apple's **StoreKit 2** only the information required to unlock paid features (entitlement status, transaction verification result). Payment details, your Apple ID, and billing information are handled by Apple and are **not** accessible to the App or the developer.

### 3.5 Sharing to Instagram

If you tap "Open Instagram" or "To Stories", the App passes the rendered image to Instagram via the system pasteboard (`UIPasteboard`) and the documented `instagram-stories://share` URL scheme. From that moment on, the data is handled by Instagram under Instagram's privacy policy. The App itself does not transmit anything over the network.

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

The App does not share photos or any data derived from them with third parties (other than the explicit user-initiated share to Instagram described in §3.5).

The App does **not** track you across other apps or websites (Apple's App Tracking Transparency prompt is not requested and is not required).

---

## 5. System permissions

The App requests the following iOS permissions:

| Permission | Type | Why it is needed |
|---|---|---|
| **Photos (Add)** | `PHPhotoLibrary.requestAuthorization(for: .addOnly)` | Save rendered carousel frames to the "Frametell" album so you can post them from the system Photos picker inside Instagram. |
| **Photos (Read)** | `PhotosPicker` (no separate prompt on iOS 16+) | Import photos you explicitly select. The system PhotosPicker runs out-of-process; the App only sees the photos you tap. |

The App does **not** request: Location, Camera, Microphone, Contacts, Bluetooth, Local Network, Calendars, Reminders, Health, Motion, or App Tracking Transparency.

You can review or revoke the Photos permission at any time in:
**iOS Settings → Privacy & Security → Photos → Frametell**

---

## 6. Purchases (Frametell Pro)

**Frametell Pro** (product ID `com.frametell.pro`) is a **non-consumable, one-time** in-app purchase processed through Apple's **StoreKit 2**. All payments and refunds are handled by **Apple**, not by the App.

- Entitlement verification is performed locally via Apple's signed `JWS` transactions (`VerificationResult`); no developer-operated server is involved.
- You can restore your purchase at any time using the "Restore Purchase" button on the paywall screen.
- Free, non-paid functionality (square 4:5 carousel, two system fonts) remains available without payment.

---

## 7. Local data storage and deletion

| Data | Storage | Removed when |
|---|---|---|
| Onboarding flag (`hasOnboarded`) | `UserDefaults` (app container) | you uninstall the App |
| Project manifests + frame images | App sandbox (Documents) | you delete the project from History or uninstall the App |
| Rendered carousel frames | iOS Photos library, "Frametell" album | you delete the album / photos in the system Photos app |

Uninstalling the App removes all data stored by the App in its sandbox. Photos already saved into the iOS Photos library remain there because they belong to your library, not to the App.

---

## 8. Network activity

The App does **not** make direct network requests to its own or any third-party servers in normal operation.

Indirect network activity may occur through Apple system APIs that the App relies on:

- **StoreKit** — Apple may contact the App Store to load product information, perform the purchase, and validate entitlements.
- **PhotoKit** — if you use **iCloud Photos**, iOS may transparently download originals from iCloud when the App imports a photo. This is iOS behavior governed by your iCloud settings.

The App uses no custom backend, no analytics endpoint, no advertising network, and no third-party SDKs.

---

## 9. Third-party services and SDKs

**The App contains no third-party SDKs.** Only Apple system frameworks are used: SwiftUI, PhotosUI, PhotoKit, StoreKit 2, UIKit, Foundation.

The App ships with three open-source fonts under permissive licenses:

- **Cormorant Garamond** — SIL Open Font License (OFL)
- **Manrope** — SIL Open Font License (OFL)
- **JetBrains Mono** — SIL Open Font License (OFL)

These fonts are bundled as resources and do not perform any network or telemetry activity.

No: Firebase, Crashlytics, Sentry, Mixpanel, Amplitude, AppsFlyer, Adjust, Branch, Google Analytics, Meta/Facebook SDK, TikTok SDK, or any other third-party analytics, attribution, advertising, or crash-reporting library.

---

## 10. Children's privacy

The App is rated **4+** but is **not directed to children under 13** (or the equivalent minimum age in your jurisdiction). The App does not knowingly collect personal information from children. Since the App does not collect personal data from any user, no special children's data is collected either.

---

## 11. Your rights (GDPR / CCPA / similar)

The App does **not collect personal data** from you on the developer side. There is therefore no personal-data record on our side to access, correct, export, restrict, or delete.

- All on-device data can be removed by uninstalling the App and deleting the "Frametell" album from the system Photos app.
- Purchase data is held by Apple under Apple's [Privacy Policy](https://www.apple.com/legal/privacy/).
- For any privacy-related question, contact us at [vrnrelax@gmail.com](mailto:vrnrelax@gmail.com). You also have the right to lodge a complaint with your local data protection authority.

---

## 12. Changes to this Policy

We may update this Privacy Policy from time to time. The "Last updated" date at the top reflects the date of the latest revision. Material changes will be reflected by updating that date.

---

## 13. Contact

For privacy-related inquiries:
[vrnrelax@gmail.com](mailto:vrnrelax@gmail.com)
