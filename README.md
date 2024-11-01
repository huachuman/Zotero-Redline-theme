# Zotero Redline (functional Zotero theme)
Zotero 7 is pretty, but it doesn't make the best use of your screen space. If you prefer getting work done over feeling pretty, and making the most out of your pixels, try this compact, functional Zotero theme.

Currently designed for dark mode.

## Features:
- generally reduced wasted space
- item hover and select effects
  - slight text zoom
  - darker background
  - red background for selected
- Truncated text cell shade (instead of ellipses)
- shorter titlebar height
- wider tabs
- grow + zoom text on tabs on hover
- smooth transition effects
- shorter toolbar
- compact collections and items pane
- fade collections when not focused
- Franklin Gothic font for compact text display
- more to come

Note: keep in mind you can adjust font size in Zotero's View menu

## Modding Zotero:
If you want further customization, here are the steps to get DevTools and use the Element Picker to edit almost anything you want. These are the steps for Windows. If someone knows the steps for other platofrms please let me know.

Create a new shortcut on your desktop or elsewhere (right click > new > shortcut) and paste this: 

"C:\Program Files\Zotero\zotero.exe" -ZoteroDebugText -jsdebugger

You may have to adjust the path for your installation. But keep the quotations marks. Save it and launch the shortcut.

Zotero with throw some warnings up, just say ok and let it load. You'll see the DevTools window appear along with Zotero now.

If you're not sure how this works, the element picker is at the top left ![image](https://github.com/user-attachments/assets/cb0b1f74-2ce2-4088-aee7-a6d62189973d). Click that and the Inspector will highlight the item's css. You can play with the css on the right panel here, under "Rules," and get the selectors for modding by copying the text above the properties (usually starts with a '.' or a '#'. You can also get them from the Inspector window by copying the class or id. You can test modifications by editing the css directly in the Rules window, but these will disappear on restart. Paste your selector and any modifications into the userChrome.css, save and restart Zotero to see what it looks like!
