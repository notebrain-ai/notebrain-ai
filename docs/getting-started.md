# Getting Started

## Installation

### Desktop (recommended)

Download the latest desktop build from the
[GitHub Releases page](https://github.com/notebrain-ai/notebrain/releases/latest)
(or use the [notebrain.ai/download](https://notebrain.ai/download) shortcut, which
auto-detects your OS and links to the right asset):

- **macOS** — `.dmg` installer (separate Apple Silicon / Intel builds)
- **Windows** — `Setup.exe` installer, or `portable.exe` (no install needed)
- **Linux** — `.AppImage` or `.deb`

Once installed, NoteBrain auto-updates from the same release feed.

### Web

Visit [app.notebrain.ai](https://app.notebrain.ai) to use NoteBrain directly in your browser. No account required.

> Note: The web version uses IndexedDB for storage. Desktop uses your local filesystem, which is more robust for large note collections.

## Creating your first note

1. Click the **+** button in the sidebar
2. Choose a note type (Text, Kanban, Canvas, etc.)
3. Start writing

## Note types

- **Text** — Rich text with Markdown support. Toggle between WYSIWYG, split, and source modes.
- **Todo** — Task lists with checkboxes, due dates, and progress bars. Cards wrap responsively.
- **Kanban** — Drag-and-drop board with customizable columns.
- **Canvas** — Infinite whiteboard for diagrams, sketches, and visual thinking.
- **Table** — Full spreadsheet with formulas, formatting, and toolbar.
- **Gantt** — Project timeline with task bars and dependencies.
- **Mind Map** — Visual mind mapping for brainstorming.
- **Timeline** — Interactive event timeline.
- **Slides** — Markdown-based presentations. Edit slides individually, present fullscreen.
- **Audio Transcript** — Record audio or upload a file. Automatically transcribed to searchable text.

## Organizing notes

- **Folders** — Right-click in the sidebar to create folders
- **Drag and drop** — Move notes between folders by dragging
- **Tags** — Add tags to notes for cross-cutting organization
- **Wiki links** — Link between notes with `[Title](note://id)` syntax

## Search

Press `Ctrl+K` (or `Cmd+K` on macOS) to open the search overlay. Search instantly across all your notes.

## AI Chat

Open the AI panel to chat with an assistant that has context from your notes. Supports:

- **Cloud AI** — 100K free tokens, or subscribe for more
- **Own API keys** — Add your Gemini, OpenAI, or Claude key in Settings
- **Ollama** — Run AI locally for free (desktop only)

## Import

Bring your existing notes from other apps:

1. Open the sidebar menu
2. Click **Import**
3. Choose your source: Notion, Obsidian, Trilium, or Markdown folder
4. Select the `.zip` export file

## Keyboard shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+K` | Search |
| `Ctrl+B` | Bold |
| `Ctrl+I` | Italic |
| `Ctrl+Space` | AI prompt (in text editor) |
| `Ctrl+S` | Save slide edit |
| `Esc` | Exit presentation / cancel edit |
