# Redmi 13C 5G Air Resources
All files required to unlock, root and optimize HyperOS for Redmi 13C 5G (Air)

(Note : The resources in this repo are not made or modded by me, but this repo is just a collection of tools I found handy developed for Redmi 13C 5G)
(Note : This tool is only for Redmi 13C 5G (AIR) and not Redmi 13C (Gale), to check what is your system, go to settings)

Resources Included in this repo:
1. KernelSU patched init_boot.img
2. HyperOS bootloader unlock request script (does not unlock or grant fake/pseudo access, just an alternative to Xiaomi Community)
3. KernelSU APK
4. Mi/Xiaomi Unlock Tool
5. AntiLowEnd module (.zip)
6. PlayIntegrity module (.zip)

## How to use the unlock request script?
### Pre-requisites:
1. You need a valid 30+ day old Xiaomi account.
2. You need a SIM card with mobile data
3. You need to be active in the Xiaomi Comunity.
### Getting Started
1. In order to use this script, log on to the xiaomi community website through your browser.
2. Install the 'Cookie-Editor' extension for your browser (available on both chromium and gecko based browsers)
3. Open the extension and search for the 'new_bbs_serviceToken' cookie and copy it's value.
4. Now extract the HyperOS script archive and edit the token.txt
5. replace the lines, 1, 2, 3, 4 with the token you just copied.
6. Now run 4 different instances of the Python script specifying the token number as 1, 2, 3, 4.

Note : As said earlier, this script doesn't grant fake access instead just automates tasks and launches request at sharp 00:00 Chinese time.

## How to unlock after obtaining the authorization?
Note: You might not be immediately able to unlock it, as usually it requires a 168 hours or a week's wait
Note: Unlocking deletes all old user data, you might need a backup.
Note: You might encounter issues during unlock, make sure you've waited for 168 hours, if not, your time will simply be incremented
1. Enter the fastboot mode / bootloader by turning off the phone and pressing Volume Down + Power button for a while, until a orange 'FASTBOOT' appears.
2. Open the Mi Unlock app in your PC, sign in with the account used in your phone.
3. Connect your phone to the PC using the charging / data transfer USB cable.
4. Your unlock tool should recognize your device and should show the 'Unlock' button.
5. Your device should be now unlocked.

## How to root?
### Pre-requisites:
* Obtain the KernelSU patched init_boot.img (kernelsu_patched_20251002_020213.img)
* ADB and Fastboot (Google Platform Tools)
### Rooting
1. Open a terminal (command prompt or Powershell or Bash) (This step onwards, even Linux is supported)
2. Enter fastboot mode or the bootloader in your unlocked phone
3. Transfer the patched init_boot.img to your PC.
4. Enter the commands:

   `fastboot flash init_boot_a <patched_init_boot.img>`
   
   `fastboot flash init_boot_b <patched_init_boot.img>`

## Next Steps
You can install the rest modules through the KernelSU app

GOOD LUCK :)
