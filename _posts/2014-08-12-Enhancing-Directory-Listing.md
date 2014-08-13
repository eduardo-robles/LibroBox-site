---
layout: post
title: Enhancing Directory Listing
date: '2014-08-12'
---

This week I was going through the LibraryBox 'Google Groups' group and found an interesting post. The user found a way to _sytle_ the directory with some CSS magic. The post was straight forward and required very little work.

The end result was a very nice looking directory listing with a _responsive_ design to boost! This was something I had been looking for and was happy someone the time to figure this out. So let's see how to customize the _directory listing_....

First, if you'd like to do the mininum amount of work you can download the zip file containing a _pre-made theme_ [here](https://groups.google.com/forum/#!topic/librarybox/3auXF3ZWSNs).

Second, extract the zip file to your computers desktop. In the zip file you'll find folder labeled _CSS_ and a file labeled _dir-generator.php_. 

Third, copy over the files (3) in the _CSS_ folder to the folder on the USB under the `/LibraryBox/Content/css` directory. You can put the _dir-generator.php_ file in the root of the USB. _HINT: you can either use FTP to transfer the files or power down the LB and transfer the files manually_. _I used FTP_. 

Fourth, _SSH_ into your LB and copy over the _dir-generator.php_ file to the appropriate directory at `/opt/piratebox/www`. _HINT: the command as follows_ `cp /mnt/usb/dir-generator.php /opt/piratebox/www`

Fifth, exit the _SSH_ session and hit refresh or go to LB page. Check the directory and the style should be updated. Enjoy!

That's all that it takes to update the style of the directory listing. There are some limitation of course and you can read about them at the 'group's' [post](https://groups.google.com/forum/#!topic/librarybox/3auXF3ZWSNs). From my testing I've noticed a slight speed increse and of course the responsive design works great on mobile. So if you want to update the _directory listing_ you can now with some _CSS_ and editing the _dir-generator.php_ file.

-Eduardo
