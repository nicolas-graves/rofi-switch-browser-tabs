Rofi switch browser tabs
===================

This script allow to use [rofi] to switch between tabs for browsers implementing the [Chrome Debugging Protocol]. It's a fork and lighter rewrite of the [original repo], and credits should go to its author. Firefox-based browser are not supported as of v105.0 (but support will be implemented). 

#### Dependencies
- wget
- jq

#### Installation
1. Copy `switch-browser-tabs` to a location which is in your path
2. Run your browser with the option `--remote-debugging-port=9222`
3. Invoke rofi with `rofi -modi 'switch-tabs:switch-browser-tabs' -show switch-tabs`

[rofi]: https://github.com/davatorium/rofi
[original repo]: https://github.com/kevinmorio/rofi-switch-browser-tabs
[Chrome Debugging Protocol]: https://chromedevtools.github.io/devtools-protocol/
