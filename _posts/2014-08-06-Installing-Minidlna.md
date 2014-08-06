---
layout: post
title: Installing MinDLNA
date: '2014-08-06'
---

This past week I decided to try to install _MiniDLNA_ on my _LibroBox_. I got the idea after stumbling on a thread on the _LibraryBox_ Google Groups group. The installation did not seem difficult if you installed _LibraryBox_ via the "auto-install" feature. The installation is literally downloading a ZIP file and editing a single file.
So let's get to installing _MiniDLNA_ on your _LibraryBox_! Disclaimer, make sure you have an internet connection just in case someting goes wrong you can find help.

First, download the auto install zip of PirateBox [here](http://stable.openwrt.piratebox.de/auto/install_piratebox.zip)

Second, if your Librarybox is on, turn it off and unplug the USB drive and plug into your PC.

Third, in the LibraryBox USB rename the "install" folder to "old-librarybox-install" then unzip the PirateBox zip file and transfer the "install" folder to the Librarybox USB.

Fourth, in the install folder open the file "auto package" with a text editor. Remove everything but "extededRoot-minidlna" and save the file. **<--VERY IMPORTANT!! If you don't do this it may BREAK your LibraryBox**

Fifth, safely remove the USB from your PC and put it in the LibraryBox and turn it on.

Sixth, minidlna will now self install wait untill the installation finishes (about 15-20 minutes).

Seventh, after installation is complete SSH into your LibraryBox. Copy the minidlna config file to the appropriate directory. Like so..**copy this command exactly as it is!!**

`cp /opt/piratebox/src/openwrt.example.minidlna /mnt/ext/etc/config/minidlna`

Eigth, start MinDLNA like so.... **must be SSh'ed into LibraryBox**

`/etc/init.d/minidlna start`

Ninth, enjoy!!

Final thoughts:

You can edit some of the MinDLNA features by editing the following file like so... 

`vi /etc/config/minidlna`

If on step 7 you get an error minidlna may have not installed. Double check the installation or redo the installation.
And that's all it takes to get MiniDLNA installed on LibraryBox!

-Eduardo 