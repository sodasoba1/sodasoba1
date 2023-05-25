#:fontawesome-solid-circle-question:{ .th-red } Troubleshooting

??? Question "NX Titles List Dumper :fontawesome-solid-file-csv: CVS error?"

	are you getting Errors importing titles.csv?
	lets see if we can fix that.

	In NX-GIC go to `File > Settings`

	[![nxgic-settings](<img/usingnxgic/settings.jpg>)]{Settings|info}

	if you have something in the [`Installed Titles List (CSV)`]{if delete is clickable|rounded|info} path click [Delete]{delete|bottom|rounded|error}.

	then click [{==SAVE==}]{SAVE|right|rounded|success}

	??? Bug "Possible Bug"
		I recommend closing nx-gic and reopening it, this seems to be better at refreshing the changes made
		I'm not sure if this is a database issue or how nxgic saves changes made to the program

		![nxgic](<img/usingnxgic/bug/csv.png>)



	If you have followed by guide you should have titles.csv in the same folder as nx-gic 
	copy the path ++ctrl+c++

	[![nxgic](img/usingnxgic/bug/csv1.png)]{Copy the Address Bar|info}

	once again open NX-GIC go to `File > Settings`

	and paste ++ctrl+v++ the nx-gic location we have just copied into [`Installed Titles List (CSV)`]{D:\Switch Icons\NX-Game-Icon-Customizer\titles.csv|bottom|rounded|error}
	??? Bug "Possible Bug"
		I recommend closing nx-gic and reopening it, this seems to be better at refreshing the changes made
		I'm not sure if this is a database issue or how nxgic saves changes made to the program
	
		![nxgic](<img/usingnxgic/bug/csv1.1.png>)

	To Reload titles.csv Click on Auto GIC
	Hit Ok and locate the titles.csv file

	![nxgic](<img/usingnxgic/bug/csv2.png>)

	click open and titles installed should work correctly
	![nxgic](<img/usingnxgic/bug/csv3.png>)

	??? Bug "Possible Bug"
		I've noticed errors where nx-gic fails to load the csv correctly and can possibly delete the CSV file from your system
		so either have a backup or recopy the file from your SD card.
	
??? Question "How do I Delete Icons?"

	The main way to delete icons is to navigate to `SD:/atmosphere/contents/TITLEID/` then delete `icon.jpg` from that folder.

	if you want to remove *ALL* icons you can do one of two things.
	Either `Disable sys-tweak`{no} or navigate to `SD:/atmosphere/contents/` and search for `icon.jpg` or `*.jpg` and delete all the `jpgs`
	
??? Question "I've updated my firmware and now my switch won't boot"
	Has your dog :fontawesome-solid-dog:{ .color-block .th-red } or cat :fontawesome-solid-cat:{ .th-red .color-block } updated your switch and now it's not booting?
	
	* Disable all modules before updating 
	* if you have updated before doing so you can delete sys-modules 
	__(re-add them when they're updated)__
	
		or
	
	* simply delete `boot2.flag` for all modules and enable them one by one
	
	* Delete all your old themes 
	
		- `sdmc:/atmosphere/contents/0100000000001000` (qlaunch)
		- `sdmc:/atmosphere/contents/0100000000001007` (playerselect)
		- `sdmc:/atmosphere/contents/0100000000001013` (User Page)
		
??? Question "Icons are showing as GREY QUESTIONMARK :material-help-box:"
	![img](<img/error.png>) 
	
	if an installed icon is showing up as a grey questionmark that usually means the icon used is the incorrect format, this could be due to many reasons but the easiest way to fix it is by:
	
	* be sure the image is resized to _256px_{.no } x _256px_{.no }
	* The image is saved as *.jpg*{ .no } 
	* the jpg is *non-progressive*{ .no }
	* the file size **under 128kb**{ .th-red } aim for ***<ins>120kb</ins>***{ .no }