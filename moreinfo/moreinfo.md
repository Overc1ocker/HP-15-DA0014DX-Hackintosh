**More info about this laptop**

- The preinstalled SSD is a Sandisk 128GB SSD. It is **SATA** based even though it plugs into the M.2 slot! This specific SSD will not be detected in Big Sur. Use CtlnaAHCIPort kext to fix! You may also replace this with a NVME based SSD.
- The brightness keys do not work natively. A PS2 remap has been included in the SSDT-HPbrightkeys-trackpadbtns SSDT. This maps F2 and F3 to the brightness keys.
- The Trackpad buttons **DO NOT** work without a VoodooPS2 specific SSDT! This has been included.
- The WIFI card is not original. The included Realtek card **DOES NOT** work in macOS. Plus it is lacking newer WiFi technlogies. I'd recommend replacing it with a Intel or Broadcom supported wifi card (or use ethernet). For Intel wifi cards, a special *itlwm* kext is required!

- Sleep occasionally breaks. I will include the fix when I get a chance to upload.
- Cpu runs inefficiently. I used CPU friend to fix. Will include this later. LFM for this CPU is 400mhz
- Builtin HDMI port does not work properly without a config.plist mode change for con1 to hdmi. I will include the fix later.

**If you love living on the edge, the CFG LOCK on this system may be removed."**
Make sure you fully understand what you are doing before you try. DO NOT TRUST RANDOM PEOPLE ON THE INTERNET.
Hint: The "setup" EFI variable is locked, however the "CPUsetup" variable is not. Use RU.exe to edit
Set 0x3C to 0x0 to disable CFGlock
I'm not responsible for bricked computers

**If you have removed CFG lock, why not set DVMT-PreAlloc to 64mb**
This will bring your IGPU to FULL POWER!
This setting exists in the "SAsetup" EFI var (unlocked)
Set 0xDF to 0x2 for the required 64MB of memory
