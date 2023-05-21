 ![icongrabber](<img/icongrabber/ig.png>){: style="float: left"}
IconGrabber is a homebrew app that one can probably best described as an 
unofficial steamgriddb client for the Nintendo Switch.

You can search for games and then preview and download icons that you want.  

After that you can apply any icon to any installed title of your switch and replace the original. 

[]{left}

[]{left}

* [IconGrabber<br> ![](https://img.shields.io/github/downloads/Slluxx/IconGrabber/total?color=red&style=flat-square)](https://github.com/Slluxx/IconGrabber)
* [REQUIRED: An API key from steamgriddb.com](sg-api.md)
* [sys-tweak is required](sys-tweak.md)

Setup
---
once you have icongrabber on your switch load it up
> first time users will need their steamgriddb API key
 
[![icongrabber](<img/icongrabber/1.jpg>)]{First time setup needs the api key from steamgriddb|top|rounded|bounce|error}

when you *first load* Icon Grabber you will need to input your [API key from steamgriddb](sg-api.md)
[![icongrabber](<img/icongrabber/2.jpg>)]{Enter your API Key|top|rounded|bounce|warning}

once entered the setup page should show your api key,
be sure to select the icon resolution you want to use, Slluxx Does a great job of explaining which resolution you should choose.
[![icongrabber](<img/icongrabber/2.5.jpg>)]{Once Entered your API Key will show in settings|top|rounded|bounce|success}

??? Warning "Manually Setting The API Key"
	Alternatively If you are having difficulty with the api key inapp you can add it by editing the config.json file located
	on the switch SD card `SDMC:/config/icongrabber/config.json`
	![icongrabber](<img/icongrabber/switch-config.png>)
	
	simply open the json file with notepad and paste your API key in between " "
	
	then save the changes `File > Save` or ++ctrl+s++

Searching
---

Searching for icons can be done in 2 ways the easiest method is using the Search by installed titles
> if you get an error saying icon not found there isn't an icon setup for that game
> you might be able to try searching by game name using a shorter name
> *i.e: mario*

![icongrabber](<img/icongrabber/3.jpg>)

on the next page you will get a list of installed games installed
select the game you want to search for an icon of. in this example I'm searching for "New Super Mario Bros. U Deluxe"
![icongrabber](<img/icongrabber/4.jpg>)

if a title is found you should see the game name you are looking for
![icongrabber](<img/icongrabber/5.png>)

###Download
you should then get a list if icons from this list you can choose an icon you like.
![icongrabber](<img/icongrabber/6.jpg>)

once you find a suitable icon click Download you should get a small popup on the top right
[![icongrabber](<img/icongrabber/7.jpg>)]{When you download a image you will get a popup in the top right|top|rounded|bounce|success}

###Applying Icons
to apply the newly downloaded icon go back to the main page :material-alpha-b-circle:{ .btna } select Downloaded Icons > Browse downloaded Icons
[![icongrabber](<img/icongrabber/8.jpg>)]{Too apply Go back to the main menu|top|rounded|bounce|success}

> NB: from personal experience if the image downloaded is a png it doesn't usually apply and you will see a [?] instead of the desired icon

find the icon you want to apply click set as icon and find the game title you want to replace when you find the game you will see Icon saved.

[![icongrabber](<img/icongrabber/9.jpg>)]{pngs can cause image errors and icons won't show|top|rounded|bounce|error}

choose the title you want to apply the new icon to click ok :material-alpha-a-circle:{ .btna }
you will then see `Icon saved` popup in the top right
[![icongrabber](<img/icongrabber/13.jpg>)]{when you click 'Set as icon' you will get a 'Icon saved' popup in the top right|top|rounded|bounce|success}

Exit Icon grabber :fontawesome-solid-circle-plus:{ .btna }

[![icongrabber](<img/icongrabber/11.jpg>)]{+ to exit then reboot your switch|top|rounded|bounce|error}

**reboot**{ .no } your switch for the new icon to show up

[![icongrabber](<img/icongrabber/14.jpg>)]{REBOOTING will show all icon changes|bottom|rounded|bounce|success}