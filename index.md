# Privacy Policy — Wut

**Effective Date:** 2026-03-19
**Last Updated:** 2026-03-19

---

## Overview

Wut is a Chrome extension that analyzes web pages using AI to help you understand what a service is and whether it's right for you. This policy explains what data is involved, where it goes, and what we do (and don't do) with it.

The short version: Wut has no servers. We collect nothing. Everything stays on your device or goes directly to the AI service you choose.

---

## 1. Data We Collect

### API Keys

Your AI service API keys (Anthropic, OpenAI, or Google) are stored exclusively in `chrome.storage.local` on your device. They are never transmitted to any Wut-operated server, because no such server exists.

### Page URL and Body Text

When you trigger an analysis, the current page's URL and extracted body text are sent to the AI service API you have selected (Anthropic, OpenAI, or Google). This data is used solely to generate the analysis result. It is not stored by Wut beyond the local cache described below.

### Usage Records (Local Only)

The following information is stored locally on your device for caching and operational purposes:

- Domain of the analyzed page
- AI model used
- Token counts
- Timestamp of analysis

This data never leaves your device.

---

## 2. Data Transmission

Data is transmitted only in the following cases:

| Destination | When | What is sent |
|---|---|---|
| Anthropic API | When Claude Haiku is selected and analysis is triggered | Page URL, page body text |
| OpenAI API | When GPT-4o mini is selected and analysis is triggered | Page URL, page body text |
| Google Generative AI API | When Gemini Flash is selected and analysis is triggered | Page URL, page body text |

**Wut-operated servers: None.** No data is ever sent to any server owned or operated by Wut.

Each AI provider has its own privacy policy governing how they handle data sent to their APIs:

- Anthropic: https://www.anthropic.com/privacy
- OpenAI: https://openai.com/policies/privacy-policy
- Google: https://policies.google.com/privacy

---

## 3. Data Storage

All data associated with Wut is stored in `chrome.storage.local` on your device:

- **API keys** — Stored locally. Never transmitted to Wut.
- **Analysis cache** — Stored as `{ result, timestamp, url }`. Expires automatically after 24 hours.
- **User preferences** — Stored locally (e.g., selected AI model, language preference).

When you uninstall the extension, all data stored by Wut is deleted from your device automatically.

---

## 4. Third-Party Sharing

Wut does not share your data with any third party, with the following single exception:

The page URL and body text of the page you choose to analyze are sent to the AI service API you have selected. This transmission happens only when you explicitly trigger an analysis by opening the Wut popup.

Wut does not use:

- Advertising networks
- Analytics services (no Mixpanel, Google Analytics, or equivalent)
- Tracking or fingerprinting services
- Cookies of any kind

---

## 5. Permissions Explained

The extension requests the following Chrome permissions:

**`activeTab`**
Required to read the content of the currently active tab — the page you want to analyze. Access is granted only when you open the Wut popup. Wut does not monitor your browsing in the background.

**`storage`**
Required to save your API keys, analysis cache, and preferences to `chrome.storage.local` on your device.

**`scripting`**
Required to inject a script into the current page to extract its text content for analysis. This script runs only when you trigger an analysis.

---

## 6. Children's Privacy

Wut is not directed at children under the age of 13 and does not knowingly collect data from children.

---

## 7. Changes to This Policy

If this policy changes, the updated version will be published at this URL with a revised "Last Updated" date. Continued use of the extension after changes are published constitutes acceptance of the updated policy.

---

## 8. Contact

For questions about this privacy policy or data handling, contact:

**Email:** [YOUR_EMAIL]

---

## Revision History

| Date | Change |
|---|---|
| 2026-03-19 | Initial version published |
