# LLM Translator

[English](./README.md)

这个项目只有一段提示词。把下面的提示词复制到 Claude Code 或其他任何 LLM 模型即可生成完整应用。

**在线 Demo：** https://tasks.hamsterbase.com/llm-translator/

![Screenshot](./screenshot.png)

## 功能

- 支持自定义翻译模型 —— 可配置任意 OpenAI 兼容 API（base URL、key、model、temperature）。
- 支持自定义翻译模板 —— 使用 `{{text}}` / `{{source_lang}}` / `{{target_lang}}` 占位符自定义提示词,并通过标签页切换。

## 提示词

```txt
Build a single-file HTML app (Vue 3 + Tailwind via CDN, no build step) — an LLM-powered translator in neobrutalist
style: cream paper background with a black grid, thick 4–6px black borders, hard offset shadows (no border-radius),
accent colors acid-yellow / hot-orange / cobalt / pink, Archivo Black headings + JetBrains Mono body.

Features:
- User configures an OpenAI-compatible API (base URL, key, model, temperature); saved to localStorage.
- Multiple translation templates: name, source lang, target lang, custom prompt using {{text}} / {{source_lang}} /
{{target_lang}}; switch via top tabs. Default = one EN→ZH template (English prompt).
- Two-column workspace: input textarea ↔ streamed output; Ctrl/Cmd+Enter to run; copy / clear buttons.
- Right-side settings drawer with sub-tabs: API config · Templates editor (add/delete/rename, language selects, prompt
editor) · Import/Export (JSON, with or without API key, overwrite/merge on import).
- Bilingual UI (Chinese ↔ English) toggle next to Settings; locale persisted; status indicator (READY/SETUP) with
blinking dot.
- Footer: "Powered by HamsterBase Tasks" linking to https://tasks.hamsterbase.com/.
```

---

Powered by [HamsterBase Tasks](https://tasks.hamsterbase.com/)
