# StatusBarZoom-v50
Magisk module for v50, increases the size of system icons, clock and battery charge percentage.

The module installs an overlay for SystemUI statusbar. I've tested it with Android 10 v20a/v20n. 

It won't work with any other version/build due to the differences in framework-res/lge-res, as it needs to be recompiled with apktool using corresponding framework. 

In case anyone's intresting in doing so, this is the how-to guide:

	• pull \system\framework\framework-res.apk and put in the root of apktool
	• pull \system\framework\lge-res and put in root of apktool

	install frameworks:
	
		• apktool if framework-res.apk
		• apktool if lge-res.apk

	re-compile statusbarzoom:
	
		• apktool b StatusBarZoom
		
	put StatusBarZoom.apk in OP/Overlay or install using Magisk

![Alt text](Preview/Before.jpg?raw=true "Before")
![Alt text](Preview/After.jpg?raw=true "After")
