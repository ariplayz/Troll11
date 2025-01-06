# Troll11
A troll Windows 11 ISO that rickrolls you when you boot it.

# Instructions
Add a video.mp4 to the _internal folder. This will be run when you boot the image.

Download a Windows 11 ISO from Microsoft: https://www.microsoft.com/en-us/software-download/windows11

Mount this ISO and copy files to a folder. 
Delete setup.exe
Add Play_Video.exe and _internal to the folder with the ripped ISO. 
Open the autorun.inf, delete everything, and paste in this:

[AutoRun.Amd64]
open=rickroll.exe
icon=rickroll.exe,0

[AutoRun]
open=rickroll.exe
icon=rickroll.exe,0

Download AnyBurn, or a similar tool for creating ISO images from files/folders. https://www.anyburn.com/download.php
In AnyBurn, select "Create image from files/folders." and select all files in the folder with the ripped ISO.
Select DVD-DL in the bottom right, click next, put in a name for the ISO, and click create.

Now, when you burn this to a USB with Rufus or Balena Etcher and boot from it, it will automatically play your video.mp4. 

# Warning! Audio on the video only works sometimes! 
Sorry, but I don't know how to fix it. 
