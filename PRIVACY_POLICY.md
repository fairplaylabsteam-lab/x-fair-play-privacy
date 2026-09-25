# Privacy Policy for X Fair Play – AI Reply & Follow Manager

**Effective Date:** September 25, 2026  
**Last Updated:** September 25, 2026  
**Version:** 1.0.6  

---

## 🛡️ Core Commitment to User Privacy

**X Fair Play – AI Reply & Follow Manager** operates with a strict **Privacy-First & Client-Side Execution** architecture. 

We do **NOT** operate any central tracking servers, advertising networks, or analytics databases. We do **NOT** collect, sell, rent, or monetize your personal information, authentication credentials, account passwords, cookies, or browsing history.

---

## 1. Single Purpose & Description

The single purpose of **X Fair Play – AI Reply & Follow Manager** is to provide a productivity enhancement toolkit for users on X (formerly Twitter) to:
1. **Organize Following & Follower Lists:** Perform user-directed actions directly in the browser, such as unfollowing non-mutual accounts, following verified users, and managing follow lists.
2. **Draft Contextual AI Replies:** Assist users in drafting natural, context-relevant tweet replies using their own chosen AI model API key (Google Gemini, OpenAI ChatGPT, Anthropic Claude, xAI Grok, Groq, or OpenRouter).

All operations are initiated explicitly by the user and execute directly from the user's browser.

---

## 2. Information Collection, Processing & Data Flow

### A. Follow & Network Management (100% Local)
- **Local Execution:** Scanning and interacting with follow/unfollow lists is performed strictly client-side on the active X tab.
- **No Credentials Stored:** The extension relies solely on the user's active login session on `x.com`. It never reads, stores, or transmits your passwords or session tokens.
- **Local Storage Only:** Whitelist usernames, action counts, speed delays, and local logs are saved exclusively in your browser via `chrome.storage.local`.

### B. AI Reply Assistant (Direct Client-to-API Communication)
- **User-Provided API Keys:** Users provide their own personal API key for their preferred AI service (e.g. Gemini, OpenAI, Claude, Grok, Groq, OpenRouter). API keys are stored securely on the user's local machine in `chrome.storage.local`. They are NEVER sent to the extension developer or any unauthorized server.
- **Direct HTTPS Requests:** When you click an AI reply button on a tweet, the extension sends the text of that specific tweet and your selected prompt directive directly from your browser over an encrypted HTTPS connection to your chosen AI provider's official API endpoint.
- **Zero Intermediary Logging:** There is no intermediate proxy or developer server. The API response returns directly to your browser and populates the reply field.
- **No Training on Personal Data:** We do not retain, store, or train models on your tweets or replies.

### C. No Analytics or Third-Party Trackers
We do not use Google Analytics, Mixpanel, telemetry scripts, advertising trackers, or tracking pixels.

---

## 3. Chrome Permissions Used & Justifications

In strict accordance with Google Chrome Web Store Developer Program Policies, the extension requests only the minimum required permissions:

| Permission | Purpose & Strict Justification |
| :--- | :--- |
| **`storage`** | Required to save user configurations (whitelist handles, delay settings, language preference, theme mode, and user's private AI API keys) locally on the device using `chrome.storage.local`. |
| **`sidePanel`** | Required to allow users to open and pin the extension control panel in Chrome's native Side Panel alongside their active X tab for convenient multitasking. |
| **`notifications`** | Required to display native desktop alerts when a long batch action finishes or when an automatic rate-limit cooldown timer has elapsed. |
| **`tabs`** | Required to detect if an active `x.com` tab is open and to navigate to follow/profile pages when the user clicks an action shortcut. |
| **`alarms`** | Required to schedule background timers for the 40-minute rate-limit cooldown via `chrome.alarms`, ensuring countdown accuracy even when the popup or side panel is closed. |

---

## 4. Host Permissions & Justifications

| Host Permission | Purpose & Strict Justification |
| :--- | :--- |
| **`https://x.com/*`<br>`https://twitter.com/*`** | Required for the content script to display the AI Reply toolbar on tweets and to automate user-instructed follow/unfollow actions on X profile pages. |
| **`https://generativelanguage.googleapis.com/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to the official Google Gemini API using the user's personal Gemini API key. |
| **`https://api.openai.com/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to the official OpenAI API using the user's personal OpenAI API key. |
| **`https://api.x.ai/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to the official xAI Grok API using the user's personal xAI API key. |
| **`https://api.anthropic.com/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to the official Anthropic Claude API using the user's personal Claude API key. |
| **`https://api.groq.com/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to the official Groq Cloud API using the user's personal Groq API key. |
| **`https://openrouter.ai/*`** | Required to allow the browser to send user-initiated tweet reply prompts directly to OpenRouter API using the user's personal OpenRouter API key. |

*Note: The extension connects ONLY to the specific provider that the user selects and configures. If no API key is provided for a service, no requests are made to that service.*

---

## 5. Remote Code Policy Compliance

In full compliance with Chrome Manifest V3 regulations:
- **No Remote Code:** The extension does NOT execute remotely hosted scripts, `eval()`, or dynamic script tags.
- All application JavaScript, HTML, and CSS files are completely bundled within the local `.zip` package verified and distributed through the Chrome Web Store.

---

## 6. Data Security and Third-Party Disclosure

- We do **NOT** sell, rent, trade, or transfer any user data to third parties.
- We do **NOT** use or transfer user data for purposes unrelated to the stated core functionality.
- We do **NOT** determine creditworthiness or conduct user profiling.
- All communication with external AI providers uses industry-standard TLS/HTTPS encryption.

---

## 7. User Control & Data Deletion

You maintain complete control over your data:
- **Clear Data Anytime:** You can delete all locally stored logs, whitelists, and API keys at any time from the extension's **Settings** tab.
- **Instant Removal:** Uninstalling the extension permanently purges all local storage from your browser.

---

## 8. Contact & Developer Information

If you have any questions, privacy concerns, or feedback regarding this Privacy Policy, please contact the developer:

- **Developer:** Giang Le
- **Support Email:** [vfa.gianglt@gmail.com](mailto:vfa.gianglt@gmail.com)
