# HP-15-DA0014DX-Hackintosh

This is my attempt to get macOS Big Sur running on a relatively new HP 15 inch laptop. The model number is 15-DA0014DX.  

**What Works?**

- Built in audio (headphone jack and laptop speakers)
- Keyboard  
- USB ports 
- Built-in card reader (usb device)  
- Battery readout (with SMCbatterymanager kext)
- Intel 7265 wifi and bluetooth (Note: this is not the original card that came with the laptop.)
- Brightness control
- Sleep 
- Webcam  
- Headphone jack line in
- Built in Microphone
- Graphics acceleration  
- Ethernet  
- Trackpad (buttons do not work)  

**Not working**  
- Touchscreen (Don't anticipate this to work as real macs do not feature touchscreens)  
- Brightness keys on keyboard   
- Trackpad buttons  
-------------------------------------------  

**Notes**:  
- You will need a RTC (SSDT-RTC0) fix in order to get this laptop to boot ANYTHING macOS related. Just like the HP 250 G6, the RTC is disabled and cannot be enabled easily.  
See getting started with ACPI for help.   https://dortania.github.io/Getting-Started-With-ACPI/

- You will also need to compile your own SSDT-EC (precompiled does not seem to work as well). Use SSDTTIME to do this.

- You will need to add your own SMBIOS. Follow the opencore guide for more info.

- You must understand how opencore is configured before downloading. 

- The included EFI folder contains opencore 0.6.4 with all SSDTs, kexts, and drivers. The resources folder is missing which only matters if you would like a graphical selection screen.   https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html
----------------------

**Specs**  

**CPU**     Intel Kaby lake -r i5-8250u  
**GPU**     Intel UHD graphics 620  
**RAM**     12GB samsung DDR4-2400 ram (8+4gb)  
**SSD**     128GB Sandisk M.2 NVME SSD  
**WIFI**    Intel AC7265 m.2 wifi (Originally Realtek RTL8723DE)  
**Ethernet** RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller  
**Audio**   ALC236 HD audio and intel Sunrise point HDMI audio  
**Trackpad**   Synaptics PS2 trackpad and Keyboard   
**Webcam**   HP truvision USB webcam (built-in)  
**Screen**   15-inch BOE touchscreen with USB based touchscreen support (G2Touch Multi-Touch by G2TSP)  
**BIOS**  Bios revision f.33 (August 2020, Latest)
 

**Credits**
- Apple for macOS
- The OpenIntelWireless team for AirportItlwm
- CorpNewt for Propertree and Ssdttime
- Khronokernel and all contributors for the awesome dortania opencore guides
- Acidanthera and all contributors for Opencore
