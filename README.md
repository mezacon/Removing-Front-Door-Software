# Removing-Front-Door-Software
A quick guide for removing frontdoorsoftware - This anti-theft program was installed on my computer by my university. However, they failed to remove this location tracking software upon graduation, and frontdoorsoftware has since gone out of businuess. These are my findings and what I did to completely uninstall it from my system without having to reinstall windows.

    Search in the task manager for FDS, close the process.
    Delete C:\Program Files\FrontDoorSoftware
    Delete these files in system32: (Determined by create & modify dates that match the FrontDoorSoftware folder, among other things)
        RunFDS.exe
        UIQ.exe
        FDSMedia.exe
        FDSCredentialProvider.dll
         cip.dat
        wpsapi.dll
    Delete Registry Entries for HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\FrontDoorSoftware
    When attempting to uninstall Front Door Software in the control panel, windows will remove it from the program list.
    Restart the computer
    Once booted the FDS User account and popup on login screen were gone, as well as any evidence of it running.
