Rofi switch browser tabs
===================

These scripts allow to use [rofi] to switch between tabs for browsers implementing the Chrome Debugging Protocol.

#### Dependencies
- wget
- jq

#### Installation
1. Copy `chrome-switch-tabs` (the file, not the folder) to a location which is in your path
2. Run `google-chrome/chromium --remote-debugging-port=9222`
3. Invoke rofi with `rofi -modi 'chrome:chrome-switch-tabs' -show chrome`

[rofi]: https://github.com/davatorium/rofi
