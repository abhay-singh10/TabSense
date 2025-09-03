
# TabSense – Context-Aware Chrome Tab Manager

## Overview
TabIntent is a smart Chrome extension that helps you organize your browsing by capturing the intent behind every tab you open. It groups tabs by purpose, lets you manage and export your sessions, and provides a beautiful dashboard for productivity.

## Features
- **Intent Capture:** Prompt to select or enter the reason for opening each tab.
- **Dashboard:** View all tabs grouped by intent, with stats and management tools.
- **Tab Management:**
	- Rename intent groups
	- Close all tabs in a group
	- Remove individual tabs from a group (trash icon)
- **Session Export:** Download your current tab session as a JSON file for backup or sharing.
- **Dark Theme:** Modern, visually appealing interface.

## Project Structure
```
TabIntent/
├── manifest.json         # Extension configuration
├── background.js         # Background service worker
├── popup/                # Popup UI for intent capture
│   ├── popup.html
│   └── popup.js
├── dashboard/            # Dashboard interface
│   ├── dashboard.html
│   └── dashboard.js
├── styles/               # Custom styles (dark theme)
│   └── main.css
├── icons/                # Extension icons
└── README.md             # Project documentation
```

## Tech Stack
- **Chrome Extension Manifest V3**
- **HTML5, CSS3 (custom & Bootstrap 5), Font Awesome**
- **Vanilla JavaScript (ES6+)**
- **Chrome APIs:** tabs, storage, windows, runtime

## Installation
1. Clone or download this repository.
2. Open Chrome and go to `chrome://extensions`.
3. Enable "Developer mode" (top right).
4. Click "Load unpacked" and select the project folder.
5. The TabIntent icon will appear in your browser toolbar.

## Usage
- **Open a new tab:** The extension will prompt you to select an intent.
- **Popup:** Click the TabIntent icon to manually set intent for the current tab.
- **Dashboard:** Click "Open Dashboard" in the popup to view and manage all tabs.
- **Rename/Remove Tabs:** Use the rename button for groups or the trash icon next to any tab to remove it from the group and storage.
- **Export:** Use the "Export Session" button in the dashboard to download your session data.

## Author
Created and maintained by Abhay Singh.

---
© 2025 Abhay Singh. All rights reserved.
