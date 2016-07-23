# OS X on Lenovo Ideapad G510

```javascript
Only for Yosemite 10.10 and above.
```

This repository contains all the necessary patches and an autopatcher script for DSDT/SSDT's on G510.

#Guide for installing OS X

#Dump ACPI tables

Extract ACPI tables using any method from linux, windows or even mac.
Refer [this](https://github.com/RehabMan/HP-ProBook-4x30s-DSDT-Patch/wiki/How-to-patch-your-DSDT) excellent guide here by RehabMan on how to extract ACPI tables.
#Copy dumped ACPI tables

Make sure to copy the ACPI tables you extracted to a safe place accessible via your newly installed MAC OS.

#Patch DSDT & SSDT's

Git clone of Laptop_G510, create one with (in terminal):
```javascript
git clone https://github.com/crytyx/Laptop_G510.git
```
OR 

if you do not have a working internet connection, download the repo as zip (option in down-right corner) from an internet enabled pc.

This will create a Laptop_G510 folder with all the patches and autopatcher  script.

In a terminal navigate to the unpacked G510 git data and execute the following:

Make the script executable:
```javascript
chmod +x G510.sh
```
Run the script
```javascript
./G510.sh -h
```

```javascript
./G510.sh -t "target dir"
```

The script will guide you through the process.

NOTE: You must specify (--target/-t ) a target folder (containing extracted DSDT/SSDT's)


#Credits:

Laptop-DSDT: https://github.com/RehabMan/Laptop-DSDT-Patch  (for all the patches)

Pike R Alpha: https://github.com/Piker-Alpha/ssdtPRGen.sh  (for the CPUSpeedStep SSDT patch)

Dell XPS 9530: https://github.com/robvanoostenrijk/XPS9530-OSX (for the idea)
