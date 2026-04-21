# Luna Extensions — Privacy Policy

Last updated: April 21, 2026

## Summary

Luna is a family of Chrome extensions built on a simple promise: **your data stays on your device.** These extensions do not upload your files, your bookmarks, your documents, or any personally identifiable information to any server operated by Luna or any third party, except when **you** explicitly connect an integration (like your own Notion workspace) and **you** explicitly trigger the sync.

## What these extensions do

- **Luna Convert** — image conversion and duplicate detection, done locally in your browser.
- **Luna PDF** — PDF merge, split, rotate, view, summarize, and OCR, done locally in your browser.
- **Luna Clipper / Luna Library** — web-page clipping and bookmark management, stored locally. Writes to your own Notion/Obsidian/Google Sheets only when you connect them.
- **Luna Graph** — visualizes your own Notion workspace as a graph. Reads Notion via your own integration token.
- **Luna AI** — shared on-device language model runner. Downloads the model into your browser; inference runs on your hardware with zero network calls at inference time.

## What we collect

**Nothing.** No telemetry, no analytics, no crash reports, no account creation, no email capture.

## What stays local

- All input files (images, PDFs, documents) you drop into any extension.
- Your converted/output files — they download directly to your computer.
- Your clipped pages, bookmarks, tags, summaries.
- Your settings and preferences.
- Any downloaded AI model files (cached by your browser).

## What leaves your device (and only with your permission)

- **Notion connections**: if you paste a Notion integration token and choose a database, the extension sends page data directly to Notion's API. Luna has no intermediary.
- **Obsidian / Google Sheets / Google Drive connections**: similarly, data goes directly from your browser to the destination service. Luna is not in the middle.
- **OAuth flows** (Google Sheets, optional Notion): standard OAuth redirects. Tokens are stored in your browser's extension storage.
- **Web pages you explicitly clip**: Luna Clipper fetches the page content your active tab is on, at the moment you click "Clip." That fetch is done by your own browser.

## What we never do

- Send your data to Luna servers. There are no Luna servers in the data path.
- Sell, share, or rent your data.
- Profile you for advertising.
- Track your browsing outside of pages you explicitly clip.
- Require an account.

## Permissions explained

Each extension requests only the permissions necessary to function:
- `storage` — saves settings and clipped data in your browser's local storage.
- `downloads` — triggers file downloads to your chosen folder.
- `contextMenus` — adds right-click menu items for quick actions.
- `activeTab` (where used) — reads the current tab's content only when you trigger a clip.
- `identity` (Luna Clipper, Luna Graph) — launches the OAuth flow for Notion / Google when you connect them.
- `alarms` (Luna Graph) — scheduled refresh of your Notion workspace graph, runs locally.
- `host_permissions` on `api.notion.com` etc. — the extension talks directly to that service from your browser.

## AI models

When you enable AI features, the extension downloads a language model (approximately 1.2 GB for Llama-3.2-1B) from Hugging Face's public CDN into your browser's cache. Inference then runs entirely on your device via WebGPU. The model download is a one-time event; no subsequent network requests are made for AI inference.

## Children

Luna extensions are not designed for or directed at children under 13.

## Changes to this policy

Material changes will be reflected in an updated "Last updated" date at the top and announced in the extension's next release notes.

## Contact

Questions? Email: support@lunanote.com (or your preferred contact address).
