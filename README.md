# Clean UI

Declutters the Zen Browser interface for a cleaner experience.

## Features

- **Spacious bookmarks bar** — extra padding below the bookmarks toolbar
- **Gear menu icon** — replaces the hamburger menu (three lines) with a settings gear icon
- **Clean context menus** — removes rarely used entries:
  - Accessibility inspector
  - Send image via email
  - Screenshot
  - Open in container tab (bookmarks, sidebar, tab context)
  - Add to Essentials
- **No double separators** — automatically hides duplicate menu separators

## Installation

1. Open `about:profiles` in Zen → click "Open Folder" on the active profile (Default = yes)

2. Clone the repo into `chrome/zen-themes/`:

```bash
cd chrome/zen-themes/
git clone https://github.com/Scorpio-99/zen-clean-ui.git
```

3. Add the following entry to `zen-themes.json` in the profile folder (tip: the file is single-line and hard to read — use an online JSON editor):

```json
"zen-clean-ui": {
  "id": "zen-clean-ui",
  "name": "Clean UI",
  "description": "Spacious bookmarks bar, gear menu icon, decluttered context menus, no double separators.",
  "homepage": "https://github.com/Scorpio-99/zen-clean-ui",
  "author": "Scorpio-99",
  "version": "1.0.0",
  "tags": ["clean", "minimal", "context-menu", "bookmarks"],
  "createdAt": "2026-04-16",
  "updatedAt": "2026-04-16",
  "enabled": false
}
```

4. Restart Zen Browser — and toggle it on under Settings → Mods

## Customization

The `chrome.css` can be freely modified. Each section is labeled with a comment.
