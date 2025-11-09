Twitch Unfollower
A lightweight Chrome extension to batch‑unfollow channels on Twitch safely and reliably. Automates unfollow clicks with modal confirmation handling, supports a whitelist, configurable batch sizes/delays, live popup status, an options page for persistent settings, and a toolbar badge.
Features
- Batch unfollow with modal confirmation handling
- Whitelist (one username per line) to skip protected channels
- Batch size 0 = process all visible entries (except whitelist)
- Configurable click delay and confirm timeout
- Run until empty (auto-scroll + repeated batches)
- Live popup status with processed count and current channel
- Persistent settings via Options page (profiles, theme, import/export)
- Toolbar badge showing processed count and status colors
- Selector fallbacks and navigation/stop safeguards
Installation
- Clone or download the repository to a local folder.
- Prepare icons and logo (recommended: icon-16.png, icon-32.png, icon-48.png, icon-128.png, logo.png or logo.svg) and place them in the extension folder.
- Open Chrome (or Edge) and go to chrome://extensions (or edge://extensions).
- Enable Developer mode.
- Click "Load unpacked" and select the extension folder.
- Reload the extension after any file changes.
Usage & Options
- Open the extension popup from the toolbar.
- Configure Batch size, Click delay, Confirm timeout and Whitelist directly in the popup or open the Options page for persistent settings.
- Buttons:
- Start Batch — processes one batch
- Run until empty — repeatedly processes batches and auto-scrolls until no more visible unfollow buttons remain
- Stop — sets a stop flag to abort the current operation
- Options — opens the Options page in a tab
- Options page:
- Save default batch, delays, confirm timeout
- Rate‑limit profiles (Conservative / Normal / Fast)
- Theme selection (dark/light for popup/options)
- Import / Export settings JSON
Notes:
- Whitelist entries are username-only (no @ or /). Case-insensitive.
- Batch size 0 processes all currently visible, whitelist-filtered unfollow buttons. Use Run until empty with batch 0 to process the full following list (page will scroll).
- For best results, disable interfering extensions and avoid navigating away while processing.
Development & Contributing
- Files of interest:
- manifest.json
- popup.html / popup.js
- content.js
- options.html / options.js
- background.js
License
MIT — see LICENSE file for details.
