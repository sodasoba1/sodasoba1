#:material-wifi-off:{ .th-red } Offline NC-GIXC
offline is a good way to keep your nxgic folder clean and prevents it looking at the entire icon repo everytime you load up, you can manually add updates and your own icons

Download and extract NX-GIC

[![nxgic-setup](<img/usingnxgic/offline/offline0.1.png>)]{Extracted nxgic|info}

Make a new Folder Called `Main`

[![nxgic-main](<img/usingnxgic/offline/offline5.5.png>)]{Main|warning}

open nx-gic and select Work Offline 

`File > Work Offline`

[![nxgic-wrk-offline](<img/usingnxgic/offline/offline1.png>)]{Select Work Offline|info}

Now Download a release of the Game Icon Repo 

[![GitHub tag (VERT)](https://img.shields.io/github/v/tag/sodasoba1/NSW-Custom-Game-Icons?color=red&label=Download%20Latest%20Version%20(VERTICAL%20REPO)&logo=gitlfs&logoColor=white&style=flat-square)](https://github.com/sodasoba1/NSW-Custom-Game-Icons/tags)
<br>[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/sodasoba1/NSW-Custom-Game-Icons-square?color=gold&label=Download%20Latest%20Version%20%28SQUARE%20REPO%29&logo=gitlfs&logoColor=white&style=flat-square)](https://github.com/sodasoba1/NSW-Custom-Game-Icons/tags)

[![repo-ziptag](<img/usingnxgic/offline/offline2.png>)]{download the zip from the tags section|info}

Open the freshly downloaded {==:octicons-file-zip-24: zip==} and navigate into the zip

[![nxgic-open-zip](<img/usingnxgic/offline/offline3.png>)]{downloaded zip from the tags section|info}

extract or drag & drop the `Vertical` folder from Inside the zip file into the `Main` folder
inside the NX-GIC Directory

[![nxgic-settings](<img/usingnxgic/offline/offline4.png>)]{download the zip from the tags section|info}

Be sure the structure is correct inside `Main/Vertical/` folder

[![nxgic-settings](<img/usingnxgic/offline/struc.png>)]{folder structure of the /vertical folder|info}

!!! info inline end "info"
	refer to online guide for Setting up NX-Titles-Dumper if you run into and problems

Download {==[NX Titles List Dumper :octicons-download-24:](https://github.com/HamletDuFromage/nx-titles-list-dumper/releases)==} and place the .nro into the `sdmc:/Switch/` folder on the SD

load nx-titles-list-dumper from hbmenu

![TLD1](<img/usingnxgic/nxtitledump.jpg>)

press :material-alpha-a-circle:{ .btna } to dump your installed title IDs

this will place a file into `SD:/titles.csv` once it's `done` 

press :fontawesome-solid-circle-plus:{ .jello } to exit

![TLD2](<img/usingnxgic/nxtitledump2.jpg>)

once `SD:/titles.csv` is dumped

transfer titles.csv into the same folder as NX-GIC

[![gic-csv](<img/usingnxgic/offline/offline5.6.png>)]{download the zip from the tags section|info}

open nx-gic `File > Settings ` and put the csv location into `Installed Titles List (CSV)`

!!! bug inline end "1.4.0 Bug" 
	CLOSE nx-gic after clicking save then re-open it
[![nxgic-settings](<img/usingnxgic/offline/offline5.7.png>)]{I Manually add the location and click save|info}

Click {==SCAN==} and if everything was done correctly you should now see all the icons.

[![nxgic-scan](<img/usingnxgic/offline/offline6.png>)]{click scan|info}

Now you can work offline if you wish to transfer icons it's worth checking the other guide

[![nxgic-settings](<img/usingnxgic/offline/offline7.png>)]{offline repo setup|info}

adding your own icons can easily be done
keeping the file name structure:

| {==mariokart-8-deluxe==}-icon001-`[0100152000022000]`  |
| :-----------------------------------------------------:|
| {==GAME-NAME==}-iconXXX-`[titleID]`-(Optional-username)|

vertical icons start out at 600px x 900px (2:3 ratio) and **must**{ .no } to resized to 256px x 256px
save as jpg non-progressive and keep the filesize **under 120kb**{ .yes } otherwise they may not load
