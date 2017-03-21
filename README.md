# GKey

![Differences](https://raw.githubusercontent.com/Rion96/GKey/master/TOSKeyDevDone.png)

GKey is a German keyboard layout for Temple OS.
Due to limitations, GKey has no dead keys, no "´", no "§" and uses a Beta (β) instead of a "ß".
Instead of the usual AltGr key, the right and left Alt keys will serve as both Alt and AltGr keys as Temple OS doesn't really make use of Alt combos anyway. Instead of a "§" the 3 button will print an @ instead. You are free to change that to whatever you want.

GKey changes the Keyboard.HC.Z file which is important for changing the definition of scan codes and enabling the "<>|" Key, which isn't represented on US keyboards. To emulate AltGr functionality, GKey will also replace your HomeKeyPlugIns.HC.Z. So if you made changes to that, I recommend you back it up.

# Installation

[Video Guide](https://www.youtube.com/watch?v=boq_Yh6gLuE)


GKey requires a Kernel recompile.
It comes with a setup script, which should make installation on a VM fairly easy.

Here is a set of commands that should allow you to install GKey:

    Cd("T:");
    #include "Setup.HC.Z";
    
This script automates the Kernel compilation.
If you run into problems, or you want to install GKey on real hardware, you might have to compile the Kernel yourself:


Quick Runthrough on how to do BootHDIns:

Harddrive:

Press ENTER, then C, then ENTER again, then press p to probe, enter Base0, then enter Base1, then 0.

CD/DVD Drive:

Now press T, then p to probe again, enter Base0, then 0, then press Enter until done.
