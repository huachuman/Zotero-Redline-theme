# Zotero Redline (functional Zotero theme)
Make the most out of your pixels and try this compact, functional Zotero theme.

Currently designed for dark mode.

The zotero dev team seems to be very opinionated as to what we should be doing with their software, making decisions that, let's face it, often don't make sense.

This project was created to remedy that issue, and provide you with options to modify the Zotero interface using CSS. 

This theme is an example of that, and was created for personal purposes, so some bugs may exist, and some tweaks may be needed for your own preferences. Feel free to contribute or post anything in Issues!

But be careful, the Zotero team does not like you editing their software because they think it's going to confuse you, or you're going to forget you added this or something. That's a fair point, if you're a dummy. But you're not a dummy, are you? You're a grown-up, and you can experiment as much as you want.

## Features:
- generally reduced wasted space
- item hover and select effects
  - slight text zoom
  - darker background
  - red background for selected
- expanded quick search box
- shorter menu and toolbars
- wider tabs
- grow + zoom text on tabs on hover
- smooth transition effects
- allow narrower left + right panels
- compact collections pane
- fade collections pane when not focused
- truncated text cell shade (instead of ellipses)
- Archivo Narrow font for compact text display
  - get from google fonts: https://fonts.google.com/specimen/Archivo+Narrow
- more to come

Note: keep in mind you can adjust font size in Zotero's View menu

## Installation
Place the userChrome.css in:

C:\Users\User_name\AppData\Roaming\Zotero\Zotero\Profiles\YourProfile.default\chrome\

I think this location may be in Local instead of Roaming depending on your installation, but don't hold me to it.

## Modding Zotero:
If you want further customization, here are the steps to get DevTools and use the Element Picker to edit almost anything you want. These are the steps for Windows. If someone knows the steps for other platofrms please let me know.

Note that some elements are harder to style than others.

Create a new shortcut on your desktop or elsewhere (right click > new > shortcut) and paste this: 

"C:\Program Files\Zotero\zotero.exe" -ZoteroDebugText -jsdebugger

You may have to adjust the path for your installation. But keep the quotations marks. Save it and launch the shortcut.

Zotero with throw some warnings up, just say ok and let it load. You'll see the DevTools window appear along with Zotero now.

If you're not sure how this works, the element picker is at the top left ![image](https://github.com/user-attachments/assets/cb0b1f74-2ce2-4088-aee7-a6d62189973d). Click that and hover over the Zotero interface and you'll see in the Inspector window it will highlight the item's css. Click on an item in the Zotero interface to hold it steady in the Inspector. You can play with the css on the right panel here, under "Rules," and get the selectors for modding by copying the text above the properties (usually starts with a '.' or a '#'. You can also get them from the Inspector window by copying the class or id. You can test modifications by editing the css directly in the Rules window, but these will disappear on restart. Paste your selector and any modifications into the userChrome.css, save and restart Zotero to see what it looks like!
