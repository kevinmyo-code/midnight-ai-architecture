# Midnight AI — System Architecture

Public architecture page for **Midnight AI**, a voice-first agentic in-car AI companion for Android
head units (Kotlin, Jetpack Compose, Gemini Live).

Live page: https://kevinmyo-code.github.io/midnight-ai-architecture/

This repository contains **only the published architecture page**. The application source is in a
separate private repository; source and a demo are available on request.

## Contents

| Path | Purpose |
|---|---|
| `index.html` | The whole page — markup, styles, diagram definition, pan/zoom logic |
| `vendor/mermaid.min.js` | Mermaid 11.4.1, vendored so the page has no external runtime dependency |

## Why mermaid is vendored

The diagram renders client-side. Pinning and committing the library rather than loading it from a
CDN means the page keeps working unchanged regardless of what happens to any third-party host — it
is linked from a resume and needs to stay up.

## Local preview

```
python -m http.server 8899
```

Then open <http://localhost:8899/>.
