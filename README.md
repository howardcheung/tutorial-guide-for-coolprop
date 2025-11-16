# Quick guide for CoolProp
This document is written for non-programmers for their uses of [CoolProp](https://coolprop.org/coolprop/wrappers/Excel/index.html) for humidity and refrigerant property calculation quickly

# Use of CoolProp with Microsoft Excel in Windows

## Demonstration of Humidity Property Calculation
To calculate web-bulb temperature in degree Celcius with an air dry-bulb temperature at 26 degree Celcius and 60% relative humidity, after installation, do the following in Microsoft Excel,

<p align="center">
<img src="/Animation01.gif" width="500">
</p>

This operation says that
* You are using *HAPropsSI* formula in CoolProp to calculate psychrometric properties in Microsoft Excel
* Your '"B"' in the 1st entry implies that you want wetulb temperature in Kelvin
* Your '"T"' in the 2nd entry implies that you are entering dry-bulb temperature in Kelvin as the first input value
* Your '26+273.15' in the 3rd entry implies that you are converting 26 degree Celcius into Kelvin before entry
* Your '"R"' in the 4th entry implies that your second quantitative input is relative humidity ranged between 0 and 1
* Your '60%' in the 5th entry implies that your second input value is relative humidity at 60%
* Your '"P"' in the 6th entry implies atmospheric pressure will be entered. This is a must.
* Your last entry is 101325, implying standard atmospheric pressure at 101325 Pa
* The last reduction -273.15 converts the output from Kelvin into degree Celsius

## Demonstration of Refrigerant Property Calculation
To calculate saturation pressure of refrigerant "HFC-134a" at 26 degree Celcius, after installation, do the following in Microsoft Excel,

<p align="center">
<img src="/Animation02.gif" width="500">
</p>

This operation says that
* You are using *PropsSI* formula in CoolProp to calculate refrigerant properties in Microsoft Excel
* Your '"P"' in the 1st entry implies that you want pressure values in Pa
* Your '"T"' in the 2nd entry implies that you are entering temperature of the refrigerant as the first input value
* Your '26+273.15' in the 3rd entry implies that you are converting 26 degree Celcius into Kelvin before entry
* Your '"Q"' in the 4th entry implies that your second quantitative input is quality of the refrigerant, ranging from 0 to 1. 0 means saturated liquid, and 1 means saturated vapor. Anything in between implies the mass proportion of vapor in the liquid-vapor mixture.
* Your '1' in the 5th entry implies that your second input value is 1 - you are calculating as if the refrigerant is a saturated vapor.
* Your '"R134a"' in the 6th entry implies refrigerant "HFC-134a". Please turn the prefix "HFC", "HCFC", etc. into "R" and remove the "-" before using the refrigerant code in the formula.
* The last division converts the output from Pa into kPa.
* 
## Installation Procedure
To install the software, first, download the Windows installer of CoolProp [here](https://sourceforge.net/projects/coolprop/files/CoolProp/7.2.0/Installers/Windows/CoolProp_v7.2.0.0.exe/download?use_mirror=ixpeering)

Note: We are using a fixed mirror site for simplicity. If needed, you can go to [here](https://sourceforge.net/projects/coolprop/files/CoolProp/) to find a more appropriate mirror site to download the Windows installer.

Run the downloaded .exe file with administrator access for proper installation. To do so, right-click at the downloaded file and click "Run as administrator".

When you run the downloaded .exe file, you may encounter "Windows protected your PC" notice. Please click "More Info and "Run Anyway" to execute the installer.

<p align="center">
<img src="/Screenshot 2025-11-16 211402.png" width="500">
</p>

Once you run the executable, you will see this page.

<p align="center">
<img src="/Screenshot 2025-11-16 211727.png" width="500">
</p>

You *only* choose other options if you 
* know that your Microsoft Office is a 32-bit software from the good old days. Select "Make the 32 bit stdcall library the default CoolProp.dll"
* know that you are buying a different Microsoft Office that is under *arm64* architecture

Click "Next". You may see something like

<p align="center">
<img src="/Screenshot 2025-11-16 212000.png" width="500">
</p>

If you do, click "Skip this file (not recommended)". Open your Microsoft Excel to try it now!

## Other combinations of entries

# Disclaimer
This document is written on 2025/11/16. It does not guarantee that it would work with versions on CoolProp after this date. It is also not responsible for any damages that are done due to the use of the guide.
