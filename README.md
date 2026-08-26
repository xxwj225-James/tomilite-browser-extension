# TomiLite — Local-First AI Browser Assistant

A browser side-panel AI assistant: summarize / translate / extract the current page, clip selections into tasks & notes, and two-way sync with the TomiLite desktop app. **Bring your own API key — your data never leaves your machine.**

> This repository hosts the **release artifacts and documentation** of the extension. The source code is **closed-source** (see [LICENSE](LICENSE)) and is not published here.

## ✨ Features

- 🤖 **AI side panel** — summarize the page, extract key points, translate, ask questions about the page, analyze videos (bilibili/YouTube captions)
- 📋 **Tasks / 📝 Notes** — right-click clipping from any page; rich Markdown editor (tables, code highlighting, images); completed tasks become read-only
- 🔄 **Desktop sync** — auto two-way sync of tasks/notes when the TomiLite desktop app is running (localhost:3192)
- 🧠 **Conversation management** — token usage meter (warns at 50%), one-click compression, auto-compress
- 🔒 **Privacy first** — API key encrypted locally and sent only to the model provider you configure; tasks/notes/chats stay on your machine
- 💰 **Zero cost** — use your own API key, no middleman

## 📦 Install (developer mode — not on the stores yet)

1. Download the latest `tomilite-browser-v*.zip` from [Releases](https://github.com/xxwj225-James/tomilite-browser-extension/releases)
2. Unzip it
3. Open `chrome://extensions` (or `edge://extensions`) → enable **Developer mode** → **Load unpacked** → select the unzipped folder
4. Open the side panel → Settings → enter your LLM API key

> ⚠️ Chrome disables unpacked extensions when developer mode is turned off. A store release with auto-updates is planned.

## 🎬 Demo

<!-- TODO: add a 30-second usage GIF -->

## 🔐 Privacy

- Full policy: [PRIVACY.md](PRIVACY.md)
- API key, tasks, notes and chat history are stored only in your browser (`chrome.storage.local`), **encrypted at rest**
- The API key is sent **only** to the model provider you configure (the settings page states this explicitly)
- Ads are not based on your browsing history; affiliate links inside the extension are labeled "Sponsored"
- No account, no telemetry, no relay server

## 📄 License

**Closed-source commercial product. © 2026 TomotaVector. All rights reserved.** See [LICENSE](LICENSE). No license is granted to use, copy, modify or redistribute the source code. The release artifacts may be downloaded and installed for personal use.

## 💬 Feedback

Open a GitHub Issue or Discussion.