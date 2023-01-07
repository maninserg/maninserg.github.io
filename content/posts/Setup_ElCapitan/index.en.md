---
title: "Setting up macOS ElCapitan for development"
date: 2023-01-06T22:04:28+03:00
draft: false
author: "Segei Manin"
tags: ["MacOS", "configuration"]
categories: [Configuration]
slug: “settting-up-macos-elcapitan-for-developer”
---

## 1. Keyboard setup Motospeed Ck104 <a id="1. Keyboard setup Motospeed Ck104"></a>

Go to `System Preference/Keyboard/Modifier Keys` and select `USB Gaming Keyboard`. And we change the `Control` and `Option` keys in places so that the location of the Apple Keyboard keys matches:

{{< figure src="./2023-01-05-min.jpg" >}}


## 2. Installing Xcode and Command Line Tools <a id="2. Installing Xcode and Command Line Tools"></a>

The maximum version of XCode available for installation on MacOS ElCapitan `8.2.1`.

Download XCode and its corresponding CLT version from [Apple official website](https://developer.apple.com/download/more/)

Install `XCode 8.2.1` from `Xcode_8.2.1.xip` and then CLT from `Command_Line_Tools_macOS_10.11_for_Xcode_8.2.dmg`


## 3. Installing MacPorts and packages <a id="3. Installing MacPorts and packages"></a>

[Page with all available versions of MacPorts](https://www.macports.org/install.php#installing)

[MacPorts download link for MacOS ElCapitan](https://github.com/macports/macports-base/releases/download/v2.8.0/MacPorts-2.8.0-10.11-ElCapitan.pkg)

Run the `.pkg` file and follow the installation instructions.

[Page with available Ports](https://ports.macports.org/)

Install the following packages::

- *Development tools:*
  - `sudo port install git` [details](https://ports.macports.org/port/git/details/)
  - `sudo port install vim` [details](https://ports.macports.org/port/vim/details/)
  - `sudo port install docker` [details](https://ports.macports.org/port/docker/details/)
- *Programming languages:*
  - `sudo port install python310` [details](https://ports.macports.org/port/python310/details/)
  - `sudo port install py310-setuptools` [details](https://ports.macports.org/port/py310-setuptools/details/)
  - `sudo port install nodejs18` [details](https://ports.macports.org/port/nodejs18/details/)
  - `sudo port install php82` [details](https://ports.macports.org/port/php82/details/)
  - `sudo port install ruby31` [details](https://ports.macports.org/port/ruby31/details/)
  - `sudo port install go` [details](https://ports.macports.org/port/go/details/)
- *Databases:*
  - `sudo port install sqlite3` [details](https://ports.macports.org/port/sqlite3/details/)
  - `sudo port install mysql57` [details](https://ports.macports.org/port/mysql57/details/)
  - `sudo port install postgresql15` [details](https://ports.macports.org/port/postgresql15/details/)
  - `sudo port install mariadb` [details](https://ports.macports.org/port/mariadb/details/)
  - `sudo port install redis` [details](https://ports.macports.org/port/redis/details/)
- *Web-серверы:*
  - `sudo port install apache2` [details](https://ports.macports.org/port/apache2/details/)
  - `sudo port install nginx` [details](https://ports.macports.org/port/nginx/details/)
- *Development environments:*
  - `sudo port install Arduino` [details](https://ports.macports.org/port/Arduino/details/)
- *Network tools:*
  - `sudo port install curl` [details](https://ports.macports.org/port/curl/details/)
  - `sudo port install nmap` [details](https://ports.macports.org/port/nmap/details/)
  - `sudo port install wireshark3` [details](https://ports.macports.org/port/wireshark3/details/)
  - `sudo port install elinks` [details](https://ports.macports.org/port/elinks/details/)
- *Video tools:*
  - `sudo port install youtube-dl` [details](https://ports.macports.org/port/youtube-dl/details/)
  - `sudo port install ffmpeg` [details](https://ports.macports.org/port/ffmpeg/details/)
  - `sudo port install VLC` [details](https://ports.macports.org/port/VLC/details/)
- *System Utilities:*
  - `sudo port install htop` [details](https://ports.macports.org/port/htop/details/)
  - `sudo port install neofetch` [details](https://ports.macports.org/port/neofetch/details/)
  - `sudo port install nnn` [details](https://ports.macports.org/port/nnn/details/)
- *Graphics tools:*
  - `sudo port install gimp2` [details](https://ports.macports.org/port/gimp2/details/)
  - `sudo port install ImageMagick` [details](https://ports.macports.org/port/ImageMagick/details/)


## 4. Installing Chrome and Firefox browsers <a id="4. Installing Chrome and Firefox browsers"></a>

The available version of Google Chrome for MacOS ElCapitan is `102.0.5005.63`. Download from [Google official website](https://google-chrome.en.uptodown.com/mac/download/62632406). And install from the downloaded file `google-chrome-102-0-5005-63.pkg`.

The available version of Firefox for MacOS ElCapitan is `78.15.0esr`. Download from [Firefox official website](https://ftp.mozilla.org/pub/firefox/releases/78.15.0esr/mac/ru/) - Russian version, [Firefox official website](https://ftp.mozilla.org/pub/firefox/releases/78.15.0esr/mac/en-US/) - English version. Install from the downloaded image `Firefox 78.15.0esr_ru.dmg` or `Firefox 78.15.0esr_en_US.dmg`

Install extensions for Firefox `RuTracker - official plugin (access, etc.)`, `AdBlocker Ultimate`, `Print Edit WE`, `SingleFile`, `TWP - Translate Web Pages`


## 5. Installing VirtualBox and Virtual Machines <a id="5. Installing VirtualBox and Virtual Machines"></a>

Available version of VirtualBox for MacOS ElCapitan `6.1.40`, download it from [official website](https://www.virtualbox.org/wiki/Download_Old_Builds_6_1).

Install the following OS images `debian-live-11.5.0-amd64-cinnamon.iso`, `CentOS-7-x86_64-NetInstall-2009.iso`, `kali-linux-2022.3-installer-netinst-amd64.iso`, `ubuntu-22.04.1-live-server-amd64`.

For virtual machines select the following options:

{{< figure src="./2023-01-06-min.jpg" >}}
{{< admonition type=note title="Note" open=true >}}
**KaliLinux requires 80GB hard drive**
{{< /admonition >}}



## 6. Install Visual Studio Code <a id="6. Install Visual Studio Code"></a>

Available version of Visual Studio Code for MacOS ElCapitan `1.74.2`, download it from [official site](https://code.visualstudio.com/Download).

Unzip the zip archive and copy the application to `Applications`


## 7. Install MAMP <a id="7. Install MAMP"></a>

Available version of MAMP for MacOS ElCapitan `5.7`, download it from [official site](https://www.mamp.info/en/downloads/older-versions/), there are also older versions of MAMP.
[Download link for MAMP 5.7](https://downloads.mamp.info/MAMP-PRO/releases/5.7/MAMP_MAMP_PRO_5.7.pkg)

## 8. Setting up GitHub <a id="8. Setting up GitHub"></a>

```bash
# Generate ssh-key
ssh-keygen -t rsa -b 4096 -C "manin.serg@mail.com"

# Copy public key to clipboard
pbcopy ~/.ssh/id_rsa.pub
```

Add a new ssh key to GitHub in `Profile/Settings/SSH and GPG keys/New SSH key`. Paste the copied public key from the clipboard and give it a name.

Testing the connection using ssh keys:

```bash
ssh -T git@github.com
```

Set up `git`:

```bash
git config --global user.name "Sergei Manin"
git config --global user.email "manin.serg@gmail.com"
git config --global github.user maninserg
git config --global color.ui true
```













