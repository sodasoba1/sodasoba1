This guide is mainly for Diffpatching option.szs to give my switchdeck theme a better
overall asthetic  look and feel.

Option.szs has to be manually patched in [[switchlayouteditor](https://github.com/FuryBaguette/SwitchLayoutEditor/releases) ![GitHub all releases](https://img.shields.io/github/downloads/FuryBaguette/SwitchLayoutEditor/total?color=red&style=flat-square)]{Github|success|top}

the patched file is then copied to `SDMC:/atmosphere/contents/0100000001000/romfs/lyt` with the other szs files

It's a little more advanced but not impossible, this guide assumes you have already installed themes and extracted
your menu files already


|  Unpatched option.szs looks un themed	  |	  This is with the patched option.szs   |
|-----------------------------------------|-----------------------------------------|
|[![unpatched](<img/diffpatch/00opt.jpg>)]{UNPATCHED|error|top}  | [![patched](<img/diffpatch/01opt.png>)]{PATCHED|success|top} |

Locate your version of _Option.szs_ on your switch: `sdmc:/themes/systemData/`

[![SDMC](<img/diffpatch/01-sdmc.png>)]{sdmc:/themes/systemData/Option.szs|info|right}

Make a copy of Option.szs to your desktop & download the diffpatch

??? Info "Option.szs missing?"
	If the szs is missing you can try extracting the menu files again in NXThemes Installer
	
	open `NXThemes > Extract home menu >` Click `Extract home menu`
	![NXThemeinstaller](<img/diffpatch/extract.jpg>)

Download [[Option-diffpatch-for-switchdeck.zip :material-download-circle:{ .bounce }](Option-diffpatch-for-switchdeck.zip)]{DOWNLOAD THE ZIP|success|Bottom}

[![unpatched](<img/diffpatch/02-opt-diff-switchdeck.png>)]{JSON-Diffpatch for Option.szs|info|right}

extract the diff patch

[![unpatched](<img/diffpatch/03-ext-diff-switchdeck.png>)]{Extract|info|right}

Open switchlayouteditor and drag option.szs into the application

[![unpatched](<img/diffpatch/04-load-option.png>)]{Drag & Drop Option.szs|info|right}


once option.szs is open a smaller window will open, we only need to load our diffpatch and not actually edit anything here.

Click `Tools` > `Load JSON patch`

[![unpatched](<img/diffpatch/05-load-diff-switchdeck.png>)]{click tools in the inner window|info|right}


locate the diffpatch on your desktop and open it:

[![unpatched](<img/diffpatch/6-open-diff-switchdeck.png>)]{Click the JSON file & Open|info|right}

once it's loaded you will get a pop up stating it's loaded

[![unpatched](<img/diffpatch/7-loaded-diff-switchdeck.png>)]{Option.szs is now patched|success|right}

now save the patched option.szs

by clicking `Save` > `Save` or using the [++ctrl+s++]{SAVE|bottom} hotkeys

[![unpatched](<img/diffpatch/8-loaded-diff-switchdeck.png>)]{patched Option.szs is saved|success|right}


paste the patched option.szs from your desktop onto the SD card

`SDMC:/atmosphere/contents/010000000001000/romfs/lyt/`

[![unpatched](<img/diffpatch/9-loaded-diff-switchdeck.png>)]{Drag & Drop or paste Option.szs into lyt folder then REBOOT|error}

This folder should have other szs files already in there.

Reboot your switch and that's it.

