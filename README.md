# rswitcher
Robin's window switcher for EWMH-compliant X11 window managers. This is my attempt to create a useful window switcher using bash. Each window is shown under the dekstop it belongs to, or under the currently active desktop if it's a sticky window. Vim-like keybinds are provided to select a window and raise it. Comes with some coloring and configuration options.

I made this script because I currently use <a href="http://www.6809.org.uk/evilwm/">evilwm</a>, and sometimes I get lost alt tabbing as there is nothing which displays the current order of the windows to alt+tab to. <a href="https://github.com/Excerion/dswitcher">dswitcher</a> is great, but I like to see what desktop the windows are on. Inspired by <a href="https://code.google.com/archive/p/superswitcher/">superswitcher</a>.

### Dependencies
- wmctrl

### Installation
- make sure you have wmctrl
- (optional) put rswitcher in you path
- (optional) add a keybinding (using your desktop manager, or xbindkeys) to run a terminal with rswitcher. I use following command: `xterm +sb -geometry 150x40 -e rswitcher`. Make sure the terminal is wide enough: at least #desktops*15, or rswitcher will exit.

### Usage
- H: move left
- J: move down
- K: move up
- L: move right
- Enter/Space: raise window
- Any other key will exit

### Customization
Some colors and options can be chosen, take a look at the first few lines.
