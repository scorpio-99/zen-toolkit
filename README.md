# Zen Toolkit (MOD)

An all-in-one Zen Browser mod that declutters the interface and gives you full control over spacing, menus, tabs, find bar, borders, dialogs, and more — with 40+ configurable settings.

> **Note:** This mod is not available in the official Zen Mods Store. It must be installed manually (see instructions below).

## Features

### Spacing
- **Bookmarks toolbar** — configurable margin (top, bottom, left, right)
- **Navigation bar** — extra margin (top, bottom)
- **URL bar** — extra inline margin

### UI Tweaks
- **Menu button icon** — choose from Gear, Sliders, Grid, Wrench, Compass, or Diamond
- **Hide double menu separators** — removes duplicate separators in all menus
- **Hide sidebar scrollbar**
- **Hide status bar**

### Context Menu
Hide individual context menu entries:
- Accessibility inspector, Send image via email, Screenshot
- "Search web for...", "View page source", "Inspect", "Save page as"
- Open in container tab (bookmarks, sidebar, tabs)
- Add to Essentials, "Send page/link to device"

### Find Bar
- **Floating style** — detached, positioned find bar with animation
- **Position** — horizontal (left, center, right) and vertical (top, bottom)
- **Max width** and **border radius** configurable
- **Padding** configurable
- **Custom background color** and **shadow** toggle
- **Hide checkboxes** — Highlight, Match case, Match diacritics, Whole words (show / hide / show only when checked)
- **Hide labels** — find status and match count

### Tabs
- **Ghost tabs** — dim unloaded tabs with configurable opacity and optional grayscale
- **Remove tab close button** — all tabs, pinned only, or don't remove

### Sleek Border
- Subtle border around URL bar and web content area
- Configurable border color

### Dialogs
- **Custom dialog style** — configurable outer margin for alert/auth dialogs

## Installation

1. Open `about:profiles` in Zen → click "Open Folder" on the active profile (Default = yes)

2. Clone the repo into `chrome/zen-themes/`:

```bash
cd chrome/zen-themes/
git clone https://github.com/Scorpio-99/zen-toolkit.git
```

3. Add the following entry to `zen-themes.json` in the profile folder (tip: the file is single-line and hard to read — use an online JSON editor):

```json
"zen-toolkit": {
  "id": "zen-toolkit",
  "name": "Zen Toolkit",
  "description": "All-in-one Zen mod: spacing, context menus, find bar, ghost tabs, sleek border, dialogs, and more.",
  "homepage": "https://github.com/Scorpio-99/zen-toolkit",
  "author": "Scorpio-99",
  "version": "1.0.1",
  "tags": ["clean", "minimal", "context-menu", "bookmarks", "find-bar", "tabs", "border"],
  "createdAt": "2026-04-16",
  "updatedAt": "2026-04-16",
  "preferences": "https://raw.githubusercontent.com/Scorpio-99/zen-toolkit/main/preferences.json",
  "enabled": false
}
```

4. Restart Zen Browser — and toggle it on under Settings → Mods

## Replaces these mods

Zen Toolkit includes the functionality of these standalone mods, so you can uninstall them:

- **Better Find Bar** — floating find bar with position and style options
- **Ghost Tabs** — dim unloaded tabs
- **Remove Tab X** — remove tab close buttons
- **Sleek Border** — subtle borders on URL bar and web content

## Reset to defaults

To reset all settings to their default values, open `about:config` in Zen, search for `mod.zen-toolkit`, and delete all matching entries. Restart Zen Browser — the defaults from `preferences.json` will be restored automatically.

## Customization

The `chrome.css` can be freely modified. Each section is labeled with a comment.
