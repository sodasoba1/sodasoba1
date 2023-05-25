#[Sys-Tweak is A collection of miscellaneous mitms.](https://github.com/p-sam/switch-sys-tweak) 

The use we need it for is intercepting the displayed game icon,
essentially it swaps out the icon shown for a installed title with an icon in our atmosphere cfw located at 

` SDMC:/atmosphere/contents/TITLEID/icon.jpg `

`FEAT_NSAM_CONTROL` : [5.1.0+] Mitm's `ns:am2`->GetReadOnlyApplicationControlDataInterface to override icon/author/version/name by title.

`FEAT_NSRO_CONTROL` : [11.0.0+] Same hook as above, but mitm target is `ns:ro`


:fontawesome-solid-link:{ .th-red }  Binary Download
---

Build [switch-sys-tweak](https://github.com/p-sam/switch-sys-tweak) or alternatively use one of the links below of a pre compiled version.

| Package Links:                                                                                                         | Tested on                               | link up? |
| ----------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |:--------:|
| [[p-sam sys-tweak github artifact](https://github.com/p-sam/switch-sys-tweak/actions)]{UP|success}                                    | HOS 16.0.0 - AMS 1.5.2 | :fontawesome-solid-check:{ .yes } |
| [[A version I posted on GBATemp](https://gbatemp.net/threads/custom-game-icons-tutorial-and-sharing-hub.574675/post-9738297)]{UP|success} |  HOS 14.1.0 - AMS 1.3.2<br>to<br>HOS 16.0.2 - AMS 1.5.2  			  | :fontawesome-solid-check:{ .yes } |
| [[16BitWonder Github Repo](https://github.com/16BitWonder/switch-sys-tweak)]{Older Version|warning}								  | Forked Version :	AMS 1.0.0		  | :fontawesome-solid-check:{ .yes } |

:fontawesome-solid-folder-tree:{ .th-red }  Sys-Tweak setup
---

You need to rename the [*[sys-tweak.nsp](https://github.com/p-sam/switch-sys-tweak/actions)* to `exefs.nsp`]{github.com/p-sam/|right|rounded|bounce|success} 

Once you've done that place `exefs.nsp` in [`SDMC:/atmosphere/contents/00FF747765616BFF`]{SD Folder location|info}
setup this folder structure and contents on your [:fontawesome-solid-sd-card:{ .mild }]{SDMC:/|info|right} card:

![laytout](<img/sys-tweak/systweak-lay.png>)


toolbox.json is a settings file so sys-tweak can be switched off and on in the homebrew menu via a homebrew toolbox
 deepsea toolbox
[`SDMC:/atmosphere/contents/00FF747765616BFF/toolbox.json`]{json location on the SD Card|info}
<pre><code>
{
  "name": "sys-tweak",
  "tid": "00FF747765616BFF",
  "requires_reboot": true
}</code></pre>

???+ Warning "***boot2.flag*** [:material-alert-decagram:{ .error }]{rename a blank txt file|right|error} should be a empty file!" 
	 
	[`SDMC:/atmosphere/contents/00FF747765616BFF/flags/boot2.flag`]{empty text file|error}
	
	`boot2`, which indicates that the program should be launched during the `boot2` process.

once you have finished your sys-tweak folder [`00FF747765616BFF`]{SD:/atmosphere/contents/00FF747765616BFF/|bottom} it should like similar to this:

??? Info inline end "Pre Setup Archive of folder structure without sys-tweak"
	Alternatively I have the toolbox.json & boot.flag files pre setup [*[here :material-download-circle:{ .bounce }](setup-00FF747765616BFF.zip)*]{Download|success} 
      
      simply copy the contents to the [*{++root++}* of your sd card :fontawesome-solid-sd-card:{ .mild }]{SDMC:/|info|right}
	
	you will still need to download and to rename the *[sys-tweak.nsp](https://github.com/p-sam/switch-sys-tweak/actions)* to `exefs.nsp`
	
[![SD-contents](<img/sys-tweak/sdcontents1.png>)]{SD:/atmosphere/contents/00FF747765616BFF/|right}

--- 

### Older Version ###

**atmosphere 0.18.0**
a pre compiled version can be found on GBATEMP to get custom icons working you will need [switch-sys-tweak](https://gbatemp.net/threads/custom-game-icons-tutorial-and-sharing-hub-no-forwarders.574675/page-10#post-9366960) `NSAM` seems to work better if that crashes try the other version