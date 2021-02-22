**More info about this laptop**

- The preinstalled SSD is a Sandisk 128GB SSD, however it is **SATA** based even though it plugs into the M.2 slot! This specific SSD will not be detected in Big Sur. Use CtlnaAHCIPort kext to fix! 
- The brightness keys do not work natively. A PS2 remap has been included in the SSDT-HPbrightkeys-trackpadbtns SSDT. This maps F2 and F3 to the brightness keys. This can be removed. 
- The WIFI card is not original. The included Realtek card **DOES NOT** work in macOS. Plus it is lacking newer WiFi technlogies. I'd recommend replacing it with a Intel or Broadcom supported wifi card (or use ethernet). For Intel wifi cards, a special *itlwm* kext is required!
