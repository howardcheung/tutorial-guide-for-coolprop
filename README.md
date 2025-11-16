# Quick guide for CoolProp
This document is written for non-programmers for their uses of [CoolProp](https://coolprop.org/coolprop/wrappers/Excel/index.html) for humidity and refrigerant property calculation quickly

# Use of CoolProp with Microsoft Excel in Windows

## Demonstration of Humidity Property Calculation
To calculate web-bulb temperature in degree Celcius with an air dry-bulb temperature at 26 degree Celcius, after installation, 

## Demonstration of Refrigerant Property Calculation

## Installation Procedure
To install the software, first, download the Windows installer of CoolProp [here](https://sourceforge.net/projects/coolprop/files/CoolProp/7.2.0/Installers/Windows/CoolProp_v7.2.0.0.exe/download?use_mirror=ixpeering)

Note: We are using a fixed mirror site for simplicity. If needed, you can go to [here](https://sourceforge.net/projects/coolprop/files/CoolProp/) to find a more appropriate mirror site to download the Windows installer.

Run the downloaded .exe file with administrator access for proper installation. To do so, right-click at the downloaded file and click "Run as administrator".

When you run the downloaded .exe file, you may encounter "Windows protected your PC" notice. Please click "More Info and "Run Anyway" to execute the installer.

<p align="center">
<img src="/figures/Screenshot 2025-11-16 211402.png" width="500">
</p>

Once you run the executable, you will see this page.

<p align="center">
<img src="/figures/Screenshot 2025-11-16 211727.png" width="500">
</p>

You *only* choose other options if you 
* know that your Microsoft Office is a 32-bit software from the good old days. Select "Make the 32 bit stdcall library the default CoolProp.dll"
* know that you are buying a different Microsoft Office that is under *arm64* architecture

Click "Next". You may see something like

<p align="center">
<img src="/figures/Screenshot 2025-11-16 212000.png" width="500">
</p>

If you do, click "Skip this file (not recommended)". Open your Microsoft Excel to try it now!

# Disclaimer
This document is written on 2025/11/16. It does not guarantee that it would work with versions on CoolProp after this date. It is also not responsible for any damages that are done due to the use of the guide.
