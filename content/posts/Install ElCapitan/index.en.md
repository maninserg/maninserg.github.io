
---
title: "Clean install of macOS El Capitan"
date: 2023-01-05T22:04:28+03:00
draft: false
author: "Segei Manin"
tags: ["MacOS", "configuration"]
categories: [Configuration]
slug: “clean-install-macos-elcapitan”
---


## 1. Downloading the macOS El Capitan Installer  <a id="1. Downloading the macOS El Capitan Installer"></a>

[Page with all available versions of MacOS on the official website](https://support.apple.com/ru-ru/HT211683)

[Mac OS El Capitan 10.11.6 Download Link](https://support.apple.com/ru-ru/HT211683)


## 2. Installing the macOS El Capitan Installer <a id="2. Установка установщика MacOS ElCapitan"></a>

Double click on the downloaded `.dmg` file. Double click on the `.pkg` file. We follow the instructions. The macOS ElCapitan installer will be installed in the `Applications` folder.


## 3. Create a bootable installer on a USB flash drive or built-in volume<a id="3. Create a bootable installer on a USB flash drive or built-in volume"></a>

The USB flash drive or other volume must have a capacity of at least 14 GB and be formatted with the `MacOS Extended (Journaled)` file system.

{{< admonition type=tip title="Tip" open=true >}}
*Instead of a USB flash drive, it is better to use a dedicated volume at the end of the computer's built-in hard drive if you later want to install only on that computer.*
{{< /admonition >}}

Open the `Terminal` application. And paste the command:

```bash
sudo /Applications/Install\ OS\ X\ El\ Capitan.app/Contents/Resources/createinstallmedia 
--volume /Volumes/MyVolume --applicationpath /Applications/Install\ OS\ X\ El\ Capitan.app
```
Where **`/Volumes/MyVolume`** is the mount path of the USB flash drive or other volume in use. Taken from `Disk Utility`.


## 4. Clean install of macOS El Capitan<a id="4. Clean install of macOS El Capitan"></a>

Turn on the computer by holding down the `⌘ Cmd` and `R` keys during boot. In the loaded `Utilites OS X` application, select `Disk Utility` and format the disk to install the system in the `MacOS Extended (Journaled)` file system.

Terminate the `Utilities OS X` application using the `Utilites OS X / Finish Utilites OS X` menu. In the menu that appears, click `Boot disk...`, select the USB flash drive with the MacOS ElCapitan installer and click `Reboot...`.

You can also run the MacOS installer on reboot by holding down the `⌥Option (Alt)` key and selecting the USB flash drive from the menu that appears.
