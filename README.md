# Zotero Redline (functional Zotero theme)
Make the most out of your pixels with this compact, functional Zotero theme.

Currently designed for dark mode.

The Zotero dev team seems to have a knack for making decisions that leave us mere mortals questioning their divine wisdom. They assure us that they've put more thought into these choices than a philosopher contemplating the meaning of life, yet we can't help but wonder if they've become a bit too enamored with their own brilliance. It's as if they've gazed into the future and determined what's best for us, even if it doesn't quite align with our puny human desires. But who are we to argue with the masterminds behind the software we've grown to love and depend on? After all, they must have a secret roadmap to success that we're just not privy to. So, let's forge ahead with our own vision, and show the Zotero dev team that sometimes, the best path forward is the one we create for ourselves, even if it means going against the grain of their mysterious ways.

This project was created to remedy this, and provide you with options to mod the Zotero interface. This theme is an example of how to do this, and was created for personal purposes, so some bugs may exist, and some tweaks may be needed for your own preferences. Feel free to contribute or post anything in Issues. I'm happy to help try and adress issues, or try and help you modify other elements.

But beware, the Zotero team isn't too keen on you tinkering with things like this. They seem to think you'll get lost in the code, forget what you've done, and end up in a state of utter confusion. While that might be a valid concern for some, fear not, my intrepid friend. This modification is foolproof. If you find yourself in over your head or decide that this isn't your cup of tea, no worries. Simply remove the userchrome file from your profile\chrome folder, and voila! You'll be back to the default setup faster than you can say "I should have listened to the Zotero team."

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

Go to your user Profile folder

Windows users: `C:\Users\User_name\AppData\Roaming\Zotero\Zotero\Profiles\user_profile.default\`

Linux (Flatpak) users: `~/.zotero/zotero/XXXXXXXX.default/`

Create a chrome folder

Place the userChrome.css file in there

Start Zotero and enjoy

Reversing the changes: simply delete the file.

## Modding Zotero:
If you want further customization, you can do two things. Explore Zotero's many css files, or use the DevTools Element Picker. I recommend you start with the Element Picker.

### 1. Tinkering with the DevTools Element Picker
These are the steps for Windows. If someone knows the steps for other platofrms please let me know.

Note that some elements are harder to style than others.

Create a new shortcut wherever you like in your files (right click > new > shortcut) and paste this: 

"C:\Program Files\Zotero\zotero.exe" -ZoteroDebugText -jsdebugger

You may have to adjust the path for your installation. But keep the quotations marks. Save it and launch the shortcut.

Zotero with throw a warning or two up, just say ok and let it load. You'll see the DevTools window appear along with Zotero now.

If you're new to the element picker, you'll find it at the top left ![image](https://github.com/user-attachments/assets/cb0b1f74-2ce2-4088-aee7-a6d62189973d). Click that and hover over the Zotero interface and you'll see in the Inspector window it will highlight the item's css. Click on an item in the Zotero interface to hold it steady in the Inspector. You can play with the css on the right panel here, under "Rules," and get the selectors for modding by copying the text above the properties (usually starts with a '.' or a '#'. You can also get them from the Inspector window by copying the class or id. You can test modifications by editing the css directly in the Rules window, but these will disappear on restart. Paste your selector and any modifications into the userChrome.css, save and restart Zotero to see what it looks like!


### 2. Exploring the open source Zotero CSS codebase
Browse the files in https://github.com/zotero/zotero/tree/main/scss

Or clone/download the code and browse this folder offline

Look at different pieces of code you'd like to adjust in your userChrome.css file.


