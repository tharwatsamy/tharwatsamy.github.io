# Privacy Policy

**Effective date:** June 6, 2026  
**Last updated:** June 6, 2026

This Privacy Policy describes how **Fit Flow** (“we,” “us,” or “our”) handles information when you use our mobile application (“the App”). Fit Flow is a fitness and workout-planning app that helps you select a training goal, follow a structured workout plan, and track your progress.

By using the App, you agree to the practices described in this policy. If you do not agree, please do not use the App.

---

## 1. Summary

- **No account required.** The App does not currently offer user registration, login, or cloud-backed user profiles.
- **Your workout data stays on your device.** Preferences, progress, and profile details are stored locally using on-device storage (Hive).
- **We download workout content from the cloud.** The App reads public workout content (goals, exercises, and plans) from Google Firebase Cloud Firestore. This content is not tied to your identity.
- **We do not sell your personal information.** We do not run advertising or behavioral tracking SDKs in the current version of the App.

---

## 2. Information We Collect

### 2.1 Information You Provide

When you use the App, you may voluntarily provide:

| Data | When collected | Purpose |
|------|----------------|---------|
| **Display name** | On first visit to the home screen (optional) | Shown on your profile and home screen. If left blank, a random default name may be assigned. |
| **Training goal** | During onboarding | Used to select an appropriate workout plan (e.g., strength, muscle building, general fitness). |
| **Weekly availability** | During onboarding | Used to match you with a plan based on how many days per week you can train (2–5+ days). |
| **Starting weights** | During workout sessions | Used to display and persist per-exercise weight values (in kilograms) for your workouts. |
| **Language preference** | During onboarding or in settings | Sets the App interface to English or Arabic. |

We do **not** currently collect:

- Email address, phone number, or password  
- Payment or billing information  
- Government ID or date of birth  
- Precise location or GPS data  
- Health platform data (e.g., Apple Health, Google Fit)  
- Photos, camera input, or contacts  
- Biometric data  

### 2.2 Information Stored Automatically on Your Device

The App stores the following locally to support its features:

| Data | Storage | Purpose |
|------|---------|---------|
| **Onboarding completion status** | On-device (Hive) | Determines whether to show onboarding or the main app. |
| **Selected workout plan** | On-device (Hive) | Stores your plan structure, exercises, sets, reps, rest times, and saved weights. |
| **Workout progress** | On-device (Hive) | Tracks completed workout slots, weekly schedule anchor, rest-day selections, and per-exercise completed set counts. |
| **First-seen date** | On-device (Hive) | Used to display “Member since” on your profile. |
| **Locale code** | On-device (Hive) | Remembers your language choice (`en` or `ar`). |

This data is associated with your installation of the App on your device, not with a remote user account.

### 2.3 Information We Receive from Third-Party Services

#### Firebase Cloud Firestore (Google)

The App connects to **Google Firebase** (`fitflow-f5158` project) to **read** workout content from Firestore collections:

- `goals` — training goal definitions  
- `exercises` — exercise library (names, descriptions, media references)  
- `plans` — structured workout plans matched to goals and availability  

These requests retrieve **app content only**. The App does **not** write your name, progress, weights, or other personal data to Firestore.

When your device communicates with Firebase, Google may process standard technical information such as your IP address, device type, operating system, and app instance identifiers as part of providing the Firebase service. See [Google’s Privacy Policy](https://policies.google.com/privacy) and [Firebase documentation](https://firebase.google.com/support/privacy) for details.

#### Google Fonts

The App uses the **Google Fonts** package to load the Inter typeface. When fonts are fetched, your device may contact Google’s servers. Google may collect information described in its privacy policy. Fonts may be cached on your device after the first download.

### 2.4 Information We Do Not Collect

Based on the current App codebase:

- **No analytics SDK** (e.g., Firebase Analytics, Crashlytics) is integrated in the mobile app at this time.  
- **No push notifications** or notification permissions are requested.  
- **No advertising** or ad-tracking frameworks are used.  
- **No backend user API** is active; configured API base URLs are placeholders and are not used to transmit user data in the current release.

---

## 3. How We Use Your Information

We use the information described above solely to:

1. **Personalize your experience** — display your name, language, and member-since date.  
2. **Deliver workout plans** — fetch and cache plan content matched to your goal and weekly availability.  
3. **Track workout progress** — remember completed sets, finished sessions, weekly scheduling, and saved weights between app launches.  
4. **Operate and improve the App** — maintain local state so you can resume where you left off.

We do not use your information for targeted advertising, automated profiling for marketing, or sale to data brokers.

---

## 4. Where Your Data Is Stored

| Data type | Location | Transmitted off-device? |
|-----------|----------|-------------------------|
| Name, progress, weights, plan, preferences | Your device (Hive local database) | **No** |
| Goals, exercises, plans (content) | Downloaded from Firebase Firestore | **Yes** (read-only content fetch) |
| Fonts | Downloaded from Google Fonts (may be cached locally) | **Yes** (font files only) |

Because personal and fitness data is stored locally:

- **Uninstalling the App** generally removes this data from your device.  
- **Switching devices** does not automatically transfer your profile or progress unless you use a future backup/sync feature.  
- **No cloud account** exists today to restore deleted local data.

---

## 5. How We Share Your Information

We do **not** sell, rent, or trade your personal information.

We share limited technical data only with service providers that help the App function:

| Recipient | What is shared | Why |
|-----------|----------------|-----|
| **Google (Firebase)** | Network requests to read Firestore content; standard service metadata | To deliver workout plan content |
| **Google (Fonts)** | Font download requests; standard service metadata | To render App typography |

We may also disclose information if required by law, regulation, legal process, or to protect the rights, safety, and security of users or the public.

---

## 6. Permissions

The App requests network access to download workout content and fonts.

**Android:** Internet access is used for Firebase and font delivery.  
**iOS:** Network access is used for the same purposes; no sensitive iOS permission prompts (camera, location, health, contacts, etc.) are used in the current version.

---

## 7. Data Retention

- **On-device data** is retained until you clear app data, reset the App’s local storage (where available), or uninstall the App.  
- **Firestore content** is cached locally as part of your plan; cached copies remain on your device until cleared or overwritten.  
- We do not maintain a central database of your personal or fitness data because no user account system is implemented.

Profile settings such as **Log Out** and **Delete Account** are present in the UI for future functionality; in the current version they do not connect to a remote account or trigger server-side deletion.

---

## 8. Your Choices and Rights

Depending on your location, you may have rights to access, correct, delete, or restrict processing of your personal information.

Because Fit Flow stores personal data **locally on your device**, you can exercise many of these rights directly:

| Action | How |
|--------|-----|
| **Change your display name** | Update it when prompted, or clear app data / reinstall (current profile editing is limited). |
| **Change language** | Use the language control during onboarding or in profile settings (when enabled). |
| **Reset your plan** | Use “Reset Plan” in profile settings when that feature is enabled, or clear local app data. |
| **Delete your data** | Uninstall the App or clear the App’s storage in your device settings. |

If you are in the **European Economic Area (EEA)**, **United Kingdom**, or **California**, you may have additional rights under GDPR or CCPA/CPRA. Contact us (see Section 12) to submit a request. Because we do not operate user accounts, we may be unable to verify or fulfill requests for data we do not possess on our servers.

---

## 9. Children’s Privacy

Fit Flow is intended for a general audience and is not directed at children under 13 (or the minimum age required in your jurisdiction). We do not knowingly collect personal information from children. If you believe a child has provided personal information through the App, contact us and we will take appropriate steps to delete locally stored data by guiding you through device-level removal, since no cloud account exists.

---

## 10. Security

We take reasonable measures to protect information handled by the App, including:

- Storing personal and fitness data in the App’s local database on your device  
- Using industry-standard HTTPS/TLS for network communication with Firebase and Google Fonts  

No method of storage or transmission is 100% secure. You are responsible for securing your device (passcode, biometrics, etc.).

---

## 11. International Data Transfers

Firebase and Google Fonts are operated by Google LLC, which may process data in the United States and other countries. If you use the App from outside those regions, your information may be transferred internationally. Google provides safeguards as described in its privacy documentation.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will revise the “Last updated” date at the top of this document. Material changes may also be communicated in the App or on our website. Continued use of the App after changes take effect constitutes acceptance of the updated policy.

---

## 13. Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy or your data, contact:

**Fit Flow**  
Email: [privacy@tharwatsamy.com](mailto:privacy@tharwatsamy.com)  

*Replace the contact email above with your official support address before publishing.*

---

## 14. Platform-Specific Notes

### Android

- Application ID (production): `com.tharwatsamy.fit_flow`  
- Application ID (development flavor): `com.tharwatsamy.fit_flow.dev`  

### iOS

- Bundle identifier follows your Xcode build configuration (e.g., `com.tharwatsamy.fitFlow` / `com.tharwatsamy.fitFlow.dev`).

---

*This policy was prepared based on a review of the Fit Flow application codebase as of June 6, 2026. Update this document when you add features such as user accounts, analytics, health integrations, cloud sync, or payment processing.*
