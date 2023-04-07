# Howto: Update OpenCore with OCAT
 This is just a quick guide, to inform newbies how to update OpenCore using OCAT.  Keep in mind:  You should do this on a backup USB stick, so that if something bad happens, your main SSD will still be bootable.  You've been warned.  

1. **Download:**  Download OCAT from https://github.com/ic005k/OCAuxiliaryTools - Click RELEASES and download the latest release for your OS.  Typically that will be OCAT_Mac.dmg. 
2. **Mount and Copy:**  After downloading the OCAT_Mac.dmg file, open and mount the DMG file, and drag the OCAT file ("OCAuxilliaryTools") to your Mac's \Applications directory. 
3. **Get past Gatekeeper security checks:**  Right-Click on the file \Applications\OCAuxilliaryTools and select OPEN.  Select "OPEN" at the 'macOS cannot verify...' prompt. 
4. OCAT opens. 
5. **All steps following assume you have a working Hackintosh with an EFI setup that's already copied to your SSD's EPS (EFI) partition.  You could also do these steps on a USB stick with an EPS (EFI) partition.**
6. In OCAT, go to **Edit/Mount ESP**.  At the Mount ESP partition prompt, select your SSD's EPS partition.  Click 'Mount and open Config.plist' and your current config.plist opens. 
7. Select **Edit/Update OpenCore and Kexts**. 
8. The 'Sync OC -> x.x.x' window appears. 
9. Click "Get the latest version of OpenCore", and click OK at the successfully updated prompt.
10. On the left side of the window, select "Select All", then "Check for Kexts updates", then "Update Kexts" (This only appears if any Kext updates are possible)
11. Click Start Sync. The window disappears and the message appears "Successfully synced to OpenCore x.x.x"; click OK.
12. Click **File/Save**.  Your EFI config.plist is now saved, updated, and valid. 
13. If the icon to the right of the floppy disk is red, click it to see and identy any problems.  Correct any problems, then save again to finalize your config.plist. 
14. All done!  Test your new EFI with the latest OpenCore in place! 
