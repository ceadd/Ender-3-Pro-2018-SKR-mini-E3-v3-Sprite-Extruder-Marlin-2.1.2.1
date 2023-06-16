# Marlin 2.1.2.1 Professional Firmware Ender 3 Pro 2018 SKR mini E3 v3 Sprite Extruder

INITIAL RELEASE: IN PROGRESS _ CHECK BACK SOON

Software:
Marlin 2.1.2.1 Stable (May 16 2023)
https://github.com/MarlinFirmware/Marlin/releases/tag/2.1.2.1
Professional Firmware pre configured for a modded Creality Ender 3 Pro 2018
Input Shaping: Enabled 40k x 40k
Pressure Advanced: Enabled (0.05)
BL Touch: Enabled
Mesh: 3x4 (9 probe points)

Hardware:
Ender 3 Pro 2018 
BigTreeTech SKR mini E3 v3 
Creality Sprite Extruder Pro 
Antclabs BL Touch v3.1
Optional: Creality CR-Touch (1:1 swap with the BL Touch 3.1)
Optional: Creality Dual Axis Upgrade Kit
Optional: 5015 blower

Note: All parts above are genuine parts, this firmware does not support knock offs. 
Please make sure everything you purchase genuine before installing this firmware, especially the BT or CR Touch.
The Dual

READ CAREFULLY!

The Creality Sprite Extruder Pro REQUIRES MODIFICATIONS to work on the older Ender 3 Pro 2018 (read below)
There are also some bed size change when making these mods, the original 235x235x250 is now 220x220x250

The Firmware:
The Pre Compiled Professional Firmware is based on the stable release of Marlin 2.1.2.1. 
Most of the optional menus are unlocked, any user customizations needed should be available in the printers menus.

Creality Sprite Extruder Install Mod:
1: Dont skip this step! 
2: When installing the Sprite Extruder Pro mount to the x axis the bottom wheel the bolt needs to be flipped around (head facing backwards) or the extruder will crash
into the right side of the x axis. Further more while not technically required you should file down that bolt a couple of mm so it doesn't stick into the 
heat block. 
Ill provide some pictures in this repo as a visual references. 
(Make sure at minimum that lower bolt is flipped or your going to have a bad time)

BL Touch
Yes, you need a BL Touch, No lol I'm not going to compile a version without it. These older printers they need all the help they can get (2023) and since the sprite
extruder natively supports it theres no reason not to have one. Because of the bed size changes I also recommend you use the mount provided in the example. You
can use the stock mount if you really want, offsets are X-36.5 Y-40, you can change them in the advanced menu on your printer but the probing wont cover the
full bed. Up too you.
Bl Touch and CR-Touch are universally interchangeable on this setup. Personally I like antclabs bl touch. This will not work with bl touch clones. 
If you have a "3d Touch" sensor it will not work.

The Bed
Like i mentioned above the bed size has changed, the original 235x235x250 is now 220x220x250. This means 220 is the absolute max size and not just printable size.
I suggest setting your slicer to 210x210x240, This seems to be a safe range in my testing. Trying to print 220 might result is skipping or damage to the stepper motors.

The Files
You want the files? Sure! Ill include the full marlin firmware for you to download and modify yourself while still providing a pre compiled version for those
who dont want to mess with visual studios or compiling firmwares. The reason I'm sharing this project is to help the community reuse these aging printers instead of 
creating more e-waste. The Sprite Extruder is a great hot end option for some, its the most affordable option for direct drive and very consumer friendly.

V6
I know what your thinking.... V6, V6, V6... "Why did you buy creality junk instead of the v6" 
Really its just personal preference, no other reason whats so ever. I liked the sprite extruder. 
This is for people who want this setup. 

WARNINGS:
DO NOT set your bed size to 225, 230 or 235... Dont. You'll damage your steppers.
I take no responsibility for any damages this firmware could cause to your 3d printer.
Always do a sanity check when installing any random firmware you find on Github.
Test every motion slowly using a tool like octoprint, verify everything functions as it should before trying a test print.


STLS:
BL Touch Mount (REQUIRED)
    x offset = -46.4
    y offset = 0
https://www.printables.com/model/432401-ender-3-s1-cr-touch-mount

5015 Cooling Duct
https://www.printables.com/model/401628-high-flow-modular-5015-cooling-duct-sprite-extrude
