# Changelog

All notable changes to NoteBrain AI will be documented in this file.

## [Unreleased]

### Added
- Multi-tab workspace with split-pane layout (open up to two panes side-by-side, each with its own tabs)
- Guest mode → account migration: prompt to move browser-stored notes into a new account on sign-up
- Mobile layout refinements across the app shell, AI chat, editor, note tree, and settings

### Changed
- Auto-updater hardening for the Electron desktop app
- Public viewer polish for shared notes
- Welcome flow and toolbar updates
- Expanded E2E coverage: wiki links, attachments, all themes, public viewer, admin panel, auth, cloud API, electron auth, security headers / rate limits

### Fixed
- About dialog now shows the actual package version (was stuck at `0.1.0` because `build/inject-env.sh` hardcoded it instead of reading `package.json`)
- Various production bugs in the site backend (mailer, dashboard, download, login, register, support views) and the Electron main process

## [0.1.16] - 2026-05-25

### Added
- Rich text editor with Markdown & WYSIWYG modes
- Canvas editor (Excalidraw whiteboard)
- Kanban board editor
- Table/spreadsheet editor (Univer Sheets)
- Todo list editor with due dates and progress tracking
- Gantt chart editor
- Mind map editor
- Timeline editor
- Slide/presentation editor (Reveal.js)
- Audio transcript editor (record or upload, auto-transcribe)
- AI chat with RAG over your notes
- Support for Gemini, OpenAI, Claude API keys
- Local Ollama integration (free, unlimited)
- Graph view for note connections
- Wiki links with backlinks
- Full-text search (Lunr.js)
- Import from Notion, Obsidian, Trilium, and markdown folders
- File attachments (images, PDFs, documents)
- Dark mode
- Desktop builds for macOS, Windows, Linux
- Web app at app.notebrain.ai
