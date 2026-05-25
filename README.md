<p align="center">
  <img src="assets/logo.png" alt="NoteBrain AI" width="80" />
</p>

<h1 align="center">NoteBrain AI — Desktop</h1>

<p align="center">
  <strong>Local-first, AI-powered knowledge management</strong><br>
  Desktop app for macOS, Windows, and Linux.
</p>

<p align="center">
  <a href="https://notebrain.ai">Website</a> &bull;
  <a href="https://app.notebrain.ai">Web App</a> &bull;
  <a href="https://github.com/notebrain-ai/notebrain-ai/releases/latest"><strong>Latest Release</strong></a> &bull;
  <a href="CHANGELOG.md">Changelog</a>
</p>

---

## Download

The desktop app is **free** on all platforms. Grab the build for your OS from the [latest release](https://github.com/notebrain-ai/notebrain-ai/releases/latest):

| Platform | Asset |
|----------|-------|
| **macOS** (Apple Silicon) | `*-arm64.dmg` |
| **macOS** (Intel) | `*-x64.dmg` |
| **Windows** | `*-Setup.exe` (installer) or `*-portable.exe` |
| **Linux** | `*.AppImage` or `*.deb` |

The [download page on notebrain.ai](https://notebrain.ai/download) auto-detects your OS and points to the right asset.

Auto-update is wired through this release feed — once installed, the app keeps itself current.

## What is NoteBrain AI?

A local-first second brain with rich text, canvas, kanban, table, todo, gantt, mind map, and timeline editors — plus AI chat grounded in your own notes (RAG). Your data stays on your device unless you opt into the Cloud plan.

Full feature tour and pricing on **[notebrain.ai](https://notebrain.ai)**.

## 100% local & private setup

NoteBrain AI Desktop can run **entirely on your machine** — no account, no cloud, no telemetry, nothing leaves your device. Two pieces to set up:

### 1. Local LLM via Ollama

Used for AI chat, RAG-grounded answers, inline AI actions, summaries, translations.

```bash
# Install Ollama from https://ollama.ai, then:
ollama pull llama3.2          # or gemma3, mistral, qwen2.5, deepseek-r1, …
ollama serve                  # keep it running (auto-starts on most installs)
```

In NoteBrain AI: **Settings → AI → Provider → Ollama** → pick your installed model. Unlimited use, no API key, no internet needed once the model is pulled.

### 2. Local Speech-to-Text

Used for audio note transcription. Models download once on first use and cache locally in IndexedDB.

In NoteBrain AI: **Settings → AI → Speech-to-text** → pick a model:

| Model | Size | Languages | Accuracy | Speed |
|-------|------|-----------|----------|-------|
| **Parakeet v3** *(recommended)* | ~600 MB | 25 European | High | High |
| Whisper Base | ~180 MB | 99+ | Moderate | Fast |
| Whisper Small | ~500 MB | 99+ | Good | Good |

> **Linux note:** local STT defaults to WebAssembly on Linux desktop (WebGPU triggers a known Electron GPU-process crash after inference). Slightly slower than WebGPU but rock-solid.

### Result

Notes, transcripts, AI queries, embeddings, semantic search — all stay on your device. No API calls, no roundtrips. Combine with the desktop app's local-filesystem storage and you have a fully offline second brain.

## About this repo

NoteBrain AI is **closed-source**. This repository exists only for:

- 📦 Publishing desktop release binaries (this is what the app auto-updater reads)
- 🐛 [Bug reports](../../issues/new?template=bug_report.yml)
- 💡 [Feature requests](../../issues/new?template=feature_request.yml)
- 📜 [Changelog](CHANGELOG.md)

There is no source code in this repository. The app is a paid SaaS with a free desktop tier; the source lives in a private repository.

## License

NoteBrain AI is proprietary software. See [LICENSE](LICENSE) for terms. Third-party components are listed in [THIRD_PARTY_LICENSES.md](https://github.com/notebrain-ai/notebrain-ai/blob/main/THIRD_PARTY_LICENSES.md) once published.

---

<p align="center">
  <a href="https://notebrain.ai">notebrain.ai</a>
</p>
