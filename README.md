# Debloat and Optimize Windows 10
## Introduction

This guide's purpose is to help you optimize windows 10 settings for better performance and disable certain privacy and telemetry options, I will try to cover everything I can, from the setup till you have an optimized debloated windows.

**Please note:** Make sure to understand what each step/option you change does as it might affect a feature you use.

### The Windows 10 Setup

- Go with your setup normally as you would till you get to the Microsoft account login screen, choose the "Offline account" option at the bottom left, then click the "Limited experience" option at the bottom left again, this will allow you to choose your user folder name instead of it being your Microsoft account email, you can always link your Microsoft account later on. I also suggest not choosing a password and instead clicking next at the password screen, this is suggested as the PC is going to restart multiple times as we install updates and drives.

- On the Privacy settings section, I suggest you disable all the options for the most privacy. You can always leave the settings you need enabled, e.g Location.

- Disable activity history. This option sends Microsoft info about websites you visit and how you use apps and services.

- Disable Cortana. This option collects a bunch of info including location, contacts and voice input.

### Updating and Installing Drivers

- Head to the Settings app then to the "Update and Security" section and check for updates and install them, this process will take a while and a couple of restarts.

- Clear your old Windows files. To do this, head to disk cleanup and tick the "Old Windows" option then click cleanup system files (You will probably not need this step if you did not install a new feature update).

- Now install your drivers, every PC is different so I cannot provide a certain link for you to download drivers from, but I can help you get them. To download your chipset drivers, google the name and model of your motherboard and you will find download links for most of the drivers you'll need from the manfucaturer's site. To download your graphics card's drivers, first determine which graphics card you have, to do this, right click on the windows icon at the bottom left of your desktop and choose "Device Manager" from the menu, then click the arrow next to "Display Adaptors" and it should tell you which graphics card you own. If your graphics card is an Nvidia card, then head to Nvidia's site and download your specific driver from there, same process goes for AMD drivers.

## Debloating Windows

### Sycnex's Script

- For this step we will use a script made by Sycnex, here is the github link for the script https://github.com/Sycnex/Windows10Debloater. You need to clone the repository, to do so click on the green "Code" button which is usually at the top of the site and then click download ZIP. Extract the ZIP and then run the "Windows10DebloaterGUI.ps1" file using powershell. It will ask you to change the execution policy, type A or Y in the powershell window then click enter. **Please note:** this poses a security risk to your PC, you should change this policy back, which we will cover how to do here.

- Click Customize Blacklist, this will open a window with most the Windows 10 apps that come preinstalled, tick the ones you want to uninstall. Please know what each app does before ticking it. After you're done customizing the blacklist you can close the window and click "Remove Bloatware with Customized Blacklist", you will know this is done when the blue powershell window says "Bloatware Removed".

- Click the following options: "Disable Cortana", "Stop Edge PDF takeover", "Disable Telemetry/Tasks", "Unpin Tiles from Start" and "Remove Bloatware Reg Keys". You can choose "Uninstall Onedrive" if you don't use it. You should also click "Install .NET v3.5" as a lot of apps and games use it.

- Close all the powershell windows you have opened and open a new one as administrator, run this command "Set-ExecutionPolicy Restricted -Force", this will change the execution policy back to restricted mode.

You can now exit all the windows you've opened.

### Not Recommended Step: More Extreme Windows Optimizer and Debloater Script

**PLEASE BEWARE:** Do not perform this step if you are not advanced enough to edit its config file and understand what each option inside it does. Please do not use default options as this DISABLES WINDOWS DEFENDER and sets your UAC level to low. If you haven't any idea what this means please skip this step.

This script is made by ChrisTitusTech and you can find it here: https://github.com/ChrisTitusTech/win10script/tree/master.

This script installs helpful programs like Adobe, Chocolatey, Notepad++, MPC-HC, and 7-Zip. It also has O&O Shutup10 CFG and Run, which is really good at eliminating privcacy and telemetry settings in Windows 10.

## The Settings App

You can go though each tab and every single option in the Windows settings app to change your PC to your liking. However, I'm going to cover the main options that you should change first.

### Privacy Tab

- In the general, speech, inking & typing personalisation and activity history sections, turn off all the options.

- In the Diagnostics & Feedback section, set the diagnostic data to Basic and turn off all the other options, then scroll down to the bottom to "Feedback Frequency" and set it to Never.

- In the Background Apps and App diagnostics section, turn their options off.

### Update and Security Tab

- Head to the "Delivery Optimization" section and turn "Allow downloads from other PCs" off. Then click advanced options and limit the update bandwidth to your liking, I personally turn it down to the lowest speed possible.

## For Gamers

- Click on the Windows Logo and type "Pointer options", then click enter and disable "Enhance pointer precision". This is the mouse acceleration option that is built into Windows. This allows you to have better muscle memory which is sometimes needed in some games.

- Go to the Settings app, then click "Gaming" and head to the "Gaming Mode" section. You should experiment with enabling or disabling it to see if you can pull more performance for your games.

- Head to the Control Panel and search for "Power Plan", then choose "High Performance". In some instances you will need to create a new power plan to choose high performance, you can do so by clicking "Create a power plan" on the left of the power options window.

## Finalization

After you're down with all these optimizations, I suggest you head to the "Disk Cleanup" app again and cleanup whatever temporary files are there to clear up your drive. Now you should be done! Enjoy your new Windows 10 PC that is optimized for the best performance!
