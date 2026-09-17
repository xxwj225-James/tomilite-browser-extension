# Tomi Browser Extension v0.2.0 — Bilingual Subtitle Translation

New feature release 🎬

## ✨ What's new

- 🌐 **Bilingual subtitle translation on video sites** — a floating button appears on video pages; click it and the translated subtitle line streams in **above** the native subtitle. You see the original AND the translation at the same time — something YouTube's built-in auto-translate (which replaces the original) can't do.
  - bilibili has **no built-in subtitle translation at all** — this brings it to every video with 字幕/AI 字幕
  - YouTube: one click instead of digging through the CC menu every video; target language is independent of your YouTube UI language
  - Works with uploader subtitles, AI 字幕 (bilibili) and CC / auto-captions (YouTube)
  - Any site with standard HTML5 captions (Vimeo, Udemy, news sites, …) works out of the box
- 🎬 **Video summaries now read captions on any site** — beyond bilibili/YouTube, the summarize feature extracts HTML5 textTracks on generic video pages, upgrading them from "title + description" to real content summaries
  - Target language configurable in Settings (8 languages), default follows the UI language
  - Skips videos whose subtitles are already in the target language — no wasted API calls
  - Per-line translation cache keeps costs low; uses the fast flash-tier model
- Settings gains a **Subtitle translation** section: master switch + target language picker (auto-saved)

## 📦 Install (developer mode — store release planned)

1. Download `tomi-browser-extension-v0.2.0.zip`
2. Unzip → `chrome://extensions` (or `edge://extensions`) → enable **Developer mode** → **Load unpacked** → select the folder
3. Open the side panel → Settings → enter your LLM API key

## 🔐 Privacy (unchanged)

- API key, tasks, notes and chat history stored only in your browser, **encrypted at rest**
- API key sent **only** to the model provider you configure
- No account, no telemetry, no relay server

## 📄 License

Closed-source commercial product. **All rights reserved.** See [LICENSE](../LICENSE).

---

## 🧩 中文摘要

- 🌐 **视频站双语字幕翻译**：视频页播放器右上出现悬浮按钮，点击后译文流式显示在原生字幕**上方**——原文译文同屏对照，这是 YouTube 内置翻译（只能二选一）做不到的
  - bilibili 完全没有字幕翻译功能，本插件补上了这个空白
  - YouTube 上免去每个视频进 CC 菜单选翻译的麻烦，一键开启，且目标语言独立于 YouTube 界面语言
  - 支持 UP 主字幕、AI 字幕（bilibili）、CC / 自动字幕（YouTube）
  - 任何带标准 HTML5 字幕的网站（Vimeo、Udemy、新闻站等）开箱即用
- 🎬 **视频总结现在任何站都能读字幕** —— bilibili/YouTube 之外，通用视频页会提取 HTML5 textTracks 字幕，从"标题+简介分析"升级为真正的视频内容总结
  - 目标语言可在设置中选择（8 种），默认跟随界面语言
  - 字幕语言与目标语言相同时自动跳过，不产生 API 费用
  - 按行缓存 + Flash 模型，费用可控
- 设置页新增「字幕翻译」区块：总开关 + 目标语言下拉，即改即存

**安装**：下载 zip → 开发者模式 → 加载已解压的扩展程序 → 设置里填自己的 API Key。
