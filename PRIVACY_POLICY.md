# Privacy Policy for X Fair Play - Quick Follow Manager

**Effective Date:** August 16, 2026  
**Last Updated:** August 16, 2026  

---

## 🛡️ Core Commitment to User Privacy

**X Fair Play - Quick Follow Manager** operates with a strict **Zero Data Collection & 100% Client-Side** policy. 

We do **NOT** collect, store, transmit, share, or sell any personal data, authentication credentials, browsing history, cookies, or sensitive information to any external server or third-party service.

---

## 1. Single Purpose Description

The sole purpose of **X Fair Play - Quick Follow Manager** is to provide a lightweight productivity management tool for users on X (formerly Twitter) to organize their following and follower lists directly in their browser. It automates user-directed actions such as:
- Unfollowing non-mutual accounts (who do not follow you back)
- Following back verified (Blue badge) accounts
- Following all accounts found in a list
- Unfollowing all following accounts

---

## 2. Information Collection and Data Usage

- **No Personal Identifiable Information (PII) Collected:** The extension does not collect usernames, passwords, authentication tokens, cookies, email addresses, IP addresses, or payment details.
- **No External Server Communication:** The extension does not communicate with any external backend servers or database tracking services. All operations are performed locally between your browser and the active X web page.
- **No Analytics or Third-Party Tracking:** We do not employ Google Analytics, telemetry scripts, advertising trackers, or tracking pixels.
- **Local Storage Only:** User configurations (such as whitelist handles, daily action limits, task delays, UI language preferences, and action logs) are stored strictly on your local machine using Chrome's built-in `chrome.storage.local` API.

---

## 3. Permissions Used & Justifications

In accordance with Google Chrome Web Store Developer Policies, the extension requests only the minimum required permissions necessary to provide its core functionality:

| Permission | Purpose & Justification |
| :--- | :--- |
| **`storage`** | Stores user settings, whitelist lists, action delay preferences, language selection, and action logs locally on the user's device via `chrome.storage.local`. |
| **`activeTab`** | Grants temporary access to the currently active X (Twitter) tab when the user interacts with the extension popup or side panel. |
| **`scripting`** | Safely executes content scripts on the user's active X tab to detect DOM user elements and trigger follow/unfollow actions upon user command. |
| **`sidePanel`** | Enables the extension interface to be pinned alongside your X browsing tab via Chrome's native Side Panel feature. |
| **`notifications`** | Sends native desktop notifications to inform the user when an action batch finishes or when a rate limit is detected while running in the background. |
| **`tabs`** | Detects if an appropriate X page (e.g. `x.com/following`) is open and allows opening or navigating to the correct target page when initiated by the user. |
| **`Host: https://x.com/*, https://twitter.com/*`** | Restricts script execution strictly to official X/Twitter domains to interact with profile lists. No other websites are accessed. |

---

## 4. Remote Code Policy Compliance

In compliance with Chrome Web Store Manifest V3 requirements:
- **No Remote Code:** The extension does NOT execute remotely hosted scripts, styles, eval, or external code.
- All application code is completely self-contained within the extension package installed from the Chrome Web Store.

---

## 5. Data Security and Third-Party Disclosure

- We do **NOT** sell, trade, rent, or transfer any user data to third parties.
- We do **NOT** use or transfer user data for purposes unrelated to the core functionality of the extension.
- We do **NOT** use or transfer user data to determine creditworthiness or for lending purposes.

---

## 6. User Control & Data Deletion

You maintain full control over your data at all times:
- You can clear all stored logs and settings at any time directly through the extension's **Settings** menu.
- Uninstalling the Extension from Chrome immediately and permanently removes all locally stored extension data from your device.

---

## 7. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect modifications in browser policies or extension enhancements. Any updates will be posted to this page with an updated "Last Updated" date.

---

## 8. Contact Us

If you have any questions, concerns, or feedback regarding this Privacy Policy, please contact us at:

- **Developer / Support Email:** [vfa.gianglt@gmail.com](mailto:vfa.gianglt@gmail.com)
