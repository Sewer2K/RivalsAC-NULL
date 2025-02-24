# RivalsAC-NULL
 Some IMPORTANT Information about this

All of these Handles relate to sys calls with their driver. Closing these handles basically removes all connections from Game to Driver, therefore disabling their anticheat
I found this by scanning through all their Handles and finding all the driver shitty threading offsets.

This is currently fully undetectable ofc since it disables the anticheat

SOOOOOOOOOOOO you don't gotta be worry about being thread safe or protect your dll. It removes all guarded regions and shit ;3

Step 1:
Open Steam and put in Marvel Rivals launch args (cmd /min /C "set __COMPAT_LAYER=RUNASINVOKER && start "" %command%")

Step 2:
Download System Informer or Process Hacker, anything that can close Handles OR Threads (RUN AS ADMIN OR THIS WONT WORK)

Step 3:
Launch Marvel rivals through steam and login and shit then go to practice range

Step 4:
GO TO SYSTEM INFORMER SEARCH FOR Marvel-Win64-Shipping.exe AND DOUBLE CLICK IT
THEN GO TO HANDLES AND CLOSE THESE HANDLES:
AcSDKThread (Full Controll | Thread):
- 4 of these Handles will popup, close all 4 if there is 3 then close all of them just make sure there isnt any of them left
RTHeartBeat (Full Controll | Thread)
- This starts with the Marvel-Win64-Shipping.exe, so just close it ez

Step 5:
Load your dll using process hacker / System Informer or injector of your choice anything will work (deadass)


CREDITS FOR THE GPU CRASH DUMPS: @BagOfWewed

if you happen to run into these GPU crash dumps:

sl_interposer.dll
sl.dlss_g.dll
sl.reflex.dll

YOU need to do is go here:

C:\Program Files (x86)\Steam\steamapps\common\MarvelRivals\Engine\Plugins\Marketplace\Streamline\Binaries\ThirdParty\Win64
