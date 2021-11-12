# mflova-chrome.steup
To use it, install google chrome and its extension called "Vimium"

### Main chrome use
|Command/shortcut| Description|
|----------------|------------|
|ctrl+t|New tab|
|ctrl+d|Create bookmark|
|ctrl+w|Close tab|
|ctrl+avpag/repag|Next or previous tab|
|ctrl+number|Chose a tab|
|ctrl+l|Select the URL bar|
|ctrl+a|Select all|
|alt+left/right arrows|Go back/forward in history|


### CVIM - Chromium-vim
How to modify main options:
In order to edit the options, go to background_scripts/options.js and modify the required options. Then go to the root of chromium-vim and run:
 - npm install
 - make
 - Go to chrome > options > more tools > extensions > load unpacked > folder to cvim
This has to be done every time this script is changed. 

Since this plugin based on Vimium does not work in google chrome new tabs, it is recommmended to install "New tab redirect" plugin and set a page like "blank.org".

General note: For websites, it is used: w<key_that_identifies_web> and for repositories is r<key_that identifies_web>. If any of these letters are capital ones, the website will be opened in a new tab.

|Command/shortcut| Description|
|----------------|------------|
| Tab/Shift+Tab | Move between the options in the menu|
| h/H | Fuzzy finder history |
| b/B | Fuzzy finder bookmarks |
| t | Fuzzy finder tabs|
|f/F|Select keywords from the website|
|mf|Opens multiple pages with f|
|p/P| Print the clipboard in the URL bar|
|Alt+Z|Reopens last closed tab|
|A/D| Move backwords/forward in history of the tab|
|Alt+A/Alt+D| Previous/Next tab|
|a/d| Scroll page down and up|
|S| Alternate between two last tabs used|

The configuration can be changed either in content_scripts/mapping.js or in background_scripts/options.js. Necessary to recompile with "npm install" and "make" whenever you change something from there.
Note: npm version 8.1.0, nodejs version 10.19.10
