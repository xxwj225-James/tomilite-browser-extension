# Privacy Policy — TomiLite Browser Extension

*Effective date: 2026-08-26*

TomiLite Browser Extension ("the extension") is designed around one principle: **your data stays on your machine**. This policy explains exactly what data the extension stores, where it is sent, and how you can delete it.

## What data the extension stores (all locally)

All persistent data is stored only in your browser's extension storage (`chrome.storage.local`):

| Data | Purpose | Where it goes |
|---|---|---|
| LLM API key | Authenticates requests to your model provider | Encrypted at rest (AES-256-GCM, key stored in a separate storage slot). Sent only to the model provider you configure in Settings |
| Provider/model settings | Your chosen provider, base URL, models | Local only |
| Tasks / Notes | Your captured and edited tasks and notes | Local only. Additionally synced to the TomiLite desktop app when it is running on the same machine (localhost:3192) |
| Daily quota counter | Free-tier AI usage limit | Local only |
| UI language | Your interface language preference | Local only |
| Ad config / click counts | Displaying ad placements and aggregate click counts | Local only (no advertising network, no tracking) |

**Chat messages are not persisted** — they exist only in memory for the current session and are lost when the side panel closes.

## Where your data is sent

1. **Your chosen LLM provider** — when you use an AI feature, the request (including the page content you asked to summarize/translate/extract) is sent directly to the model provider you configured, authenticated with your own API key. No relay server is involved.
2. **Your own TomiLite desktop app** — tasks/notes sync over `localhost:3192` only when the desktop app is running on the same machine. Nothing is sent to any external server for sync.
3. **Affiliate links** — when you click a labeled "Sponsored" link, your browser opens the advertiser's website. This is a normal navigation, not data transmission by the extension.

## Page content

The extension reads the **active page's text only when you explicitly trigger an action** (summarize, translate, extract, video analysis). The content is capped and used solely to fulfill your request via your chosen model provider. The extension does not read, record or transmit your browsing history, and runs no background collection.

## What the extension does NOT do

- ❌ No account, no registration, no telemetry
- ❌ No browsing-history-based advertising or tracking
- ❌ No cookies, no fingerprinting
- ❌ No server relay or cloud storage of your data
- ❌ No background reading of pages

## Advertising

The free tier displays two ad placements inside the extension's own UI: a sponsor line under AI answers and an affiliate recommendation card. Both are labeled "Sponsored/赞助". Advertising is **not** based on your browsing history. Click counts are stored locally for the extension owner's aggregate reporting and are not sent anywhere.

## Data deletion

- **Uninstall the extension**: Chrome/Edge removes the extension's `chrome.storage.local` data on uninstall, deleting all tasks, notes, settings and the API key.
- **Clear manually**: `chrome://extensions` → TomiLite → "Clear extension data" (or the browser's site-data clearing for the extension).

## Third-party services

The only third party involved is the **LLM model provider you choose** (e.g. DeepSeek, Qwen, Moonshot, or a custom OpenAI-compatible endpoint). Data sent to them is governed by their own terms and privacy policies. We recommend you review your provider's policy.

## Security

- API key encrypted at rest (WebCrypto AES-256-GCM)
- HTTPS used for all provider requests
- No hardcoded secrets in the extension package

## Changes to this policy

We may update this policy as features evolve. The current version is always available in this document. Material changes will be noted here.

## Contact

Questions about this policy: **xxwj225@hotmail.com**

---

# 隐私政策 — TomiLite 浏览器插件

*生效日期：2026-08-26*

TomiLite 浏览器插件（下称"本扩展"）遵循一条核心原则：**你的数据只留在你自己的设备上**。本政策说明扩展存储了哪些数据、数据会发送到哪里、以及如何删除。

## 扩展存储的数据（全部在本地）

所有持久化数据仅保存在浏览器扩展存储（`chrome.storage.local`）中：

| 数据 | 用途 | 去向 |
|---|---|---|
| LLM API Key | 向你的模型服务商发起请求的身份凭证 | 本地加密存储（AES-256-GCM，密钥单独存放）。仅发送到你配置的模型服务商 |
| 服务商/模型设置 | 你选择的服务商、Base URL、模型 | 仅本地 |
| 任务 / 笔记 | 你剪藏和编辑的任务与笔记 | 仅本地。当桌面版 TomiLite 在本机运行时，会同步到本机 localhost:3192 |
| 每日额度计数 | 免费版 AI 使用次数 | 仅本地 |
| 界面语言 | 你的语言偏好 | 仅本地 |
| 广告配置 / 点击计数 | 展示广告位与聚合点击统计 | 仅本地（无广告联盟、无追踪） |

**聊天记录不持久化**——仅存在于当前会话内存中，关闭侧栏即消失。

## 数据会发送到哪里

1. **你选择的 LLM 服务商**——使用 AI 功能时，请求（包括你要求总结/翻译/提取的页面内容）直接发送给你配置的模型服务商，使用你自己的 API Key 鉴权，**不经任何中转服务器**。
2. **你自己的 TomiLite 桌面端**——仅当桌面版在同一台机器上运行时，任务/笔记通过 `localhost:3192` 同步，不经过任何外部服务器。
3. **联盟推广链接**——点击标注"赞助/Sponsored"的链接后，浏览器打开广告主网站，这是普通网页跳转，不是扩展的数据传输。

## 页面内容

扩展**仅在你主动触发操作时**（总结、翻译、提取、视频分析）读取当前页面的文字，内容有长度上限，且仅用于通过你选择的模型服务商完成你的请求。扩展**不读取、不记录、不传输浏览历史**，无任何后台采集。

## 扩展不会做的事

- ❌ 无账号、无注册、无遥测
- ❌ 不做基于浏览历史的广告与追踪
- ❌ 无 Cookie、无指纹采集
- ❌ 无服务器中转、不在云端存储你的数据
- ❌ 不在后台读取页面

## 广告

免费版在扩展自身 UI 内展示两处广告位：AI 回答下方的赞助行、空聊天页的推广卡，均标注"赞助/Sponsored"。广告**不基于浏览历史**。点击计数仅存本地，用于扩展方聚合统计，不上传。

## 数据删除

- **卸载扩展**：Chrome/Edge 卸载扩展时会清除其 `chrome.storage.local` 数据，任务、笔记、设置与 API Key 一并删除。
- **手动清除**：`chrome://extensions` → TomiLite → 清除扩展数据（或用浏览器"清除网站数据"针对本扩展执行）。

## 第三方服务

唯一涉及的第三方是**你自行选择的 LLM 模型服务商**（如 DeepSeek、通义千问、Moonshot，或自定义 OpenAI 兼容端点）。发送给它们的数据受其自身条款与隐私政策约束，建议你阅读所选服务商的政策。

## 安全措施

- API Key 本地加密存储（WebCrypto AES-256-GCM）
- 所有服务商请求走 HTTPS
- 扩展包内无硬编码密钥

## 政策更新

随着功能演进，本政策可能更新，最新版本以本文档为准，重大变更会在此注明。

## 联系方式

对本政策的疑问：**xxwj225@hotmail.com**