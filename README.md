Rofi switch browser tabs
===================

These scripts allow to use [rofi] to switch between tabs for browsers implementing the Chrome Debugging Protocol.

#### Dependencies
- wget
- jq

#### Installation
1. Copy `switch-browser-tabs` to a location which is in your path
2. Run your browser with the option `--remote-debugging-port=9222`
3. Invoke rofi with `rofi -modi 'switch-tabs:switch-browser-tabs' -show switch-tabs`

[rofi]: https://github.com/davatorium/rofi
