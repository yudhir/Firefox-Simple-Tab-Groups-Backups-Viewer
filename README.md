# TAB Groups Viewer

A simple HTML viewer for Tab Groups backup files from the Tab Groups extension.

## Quick Start

1. **Start a local server** in this folder:
   ```bash
   python -m http.server 8000
   ```

2. **Open in browser:**
   ```
   http://localhost:8000/tab-groups-viewer.html
   ```

## Features

- **Grid View**: All groups displayed as cards with tab icons
- **Drill-down**: Click a group to see full tabs with thumbnails
- **Quick Open**: Click any favicon to open the website directly
- **Browse Backups**: Use **+1** and **←** buttons to cycle through backup files (day 01-31)
- **Stay on Group**: When switching backups, the current group view stays open so you can see changes

## Navigation

- **Groups View**: Shows all groups as cards with favicon previews
- **Group Detail**: Click a group card to see all tabs with screenshots
- **Breadcrumb**: Click "Groups" to return to the main grid view
- **File Indicator**: Current backup file name shown in header

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `n` or `→` (Right Arrow) | Next backup file (+1) |
| `p` or `←` (Left Arrow) | Previous backup file |
| Click **+1** button | Next backup file |
| Click **←** button | Previous backup file |

## Requirements

- A modern web browser
- Python (for local server) or any HTTP server

## Troubleshooting

**"File not found" error**: Make sure you're running a local HTTP server, not opening the file directly. Browsers block local file access for security.

**No tabs showing**: Check that the JSON files are in the same folder as the HTML file.
