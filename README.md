# EasyNotes

A local Markdown notes app in a single `index.html`. No build step, no dependencies, no internet needed.

## Run

- **Easiest:** open `index.html` in Chrome / Edge / Brave.
- **Or** serve it locally: `python3 -m http.server 8000` then visit http://localhost:8000

On first launch choose:
- **Open a folder on disk** – your notes are real `.md` files (Chromium browsers; File System Access API).
- **Browser storage** – works in any browser; export/import via JSON.

## Features

- Word-style rich text editor (default): toolbar, headings, lists, tasks, tables, quotes, code, links. Type `## `, `- `, `1. `, `> `, `[] ` to format as you go. Saved as plain Markdown.
- Also Source (raw Markdown), Split and Preview modes (Ctrl+E cycles)
- `[[Wikilinks]]` (with `|alias` and `#heading`), autocomplete on `[[`, backlinks, outgoing links, outline
- Images: toolbar 🖼, paste from clipboard, or drag a file into the editor. In folder mode they are saved to `attachments/` as real files; in browser mode they are kept in browser storage. Referenced as `![[name.png]]` (standard `![](path)` also works)
- Embeds: `![[Note]]` or `![[Note#Heading]]` shows another note inline (loop-safe, read-only)
- Drag and drop in the file tree to move notes and folders (links are updated); drop `.md` files from your computer onto a folder to import them
- Rename a note and links across the vault are updated
- Graph view (force-directed, drag/zoom/pan, unresolved links shown)
- `#tags` and frontmatter tags, tag browser, full-text search (`tag:x`, `path:y`)
- Quick switcher (Ctrl+O), command palette (Ctrl+P)
- Daily notes (Ctrl+D) and templates (notes in `Templates/`, with `{{title}} {{date}} {{time}}`)
- Split view: two notes at once (Ctrl+\\ or the ◫ button), side by side or stacked, draggable divider, drag tabs between panes, Alt+click any link or note to open it in the other pane. Edits show live in both panes, even for the same note
- Tabs and two split panes, dark/light theme, callouts, tables, autosave

Press `?` in the app for all shortcuts.
