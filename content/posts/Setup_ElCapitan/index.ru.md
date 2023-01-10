---
title: "Настройка MacOS ElCapitan для разработки"
date: 2023-01-06T22:04:28+03:00
draft: false
author: "Segei Manin"
tags: ["MacOS", "configuration"]
categories: [Configuration]
slug: “setup-macos-elcapitan-for-development”
---

## 1. Настройка клавиатуры Motospeed Ck104 <a id="1. Настройка клавиатуры Motospeed Ck104"></a>

Заходим в `System Preference/Keyboard/Modifier Keys`, там выбираем `USB Gaming Keyboard`. И меняем клавиши `Control` и `Option` местами, чтобы было соотвествие расположения клавиш Apple Keyboard:

{{< figure src="./2023-01-05-min.jpg" >}}


## 2. Установка XCode и Command Line Tools <a id="2. Установка XCode и Command Line Tools"></a>

Максимальная версия XCode доступная для установки на MacOS ElCapitan `8.2.1`.

Скачиваем XCode и соотвествующую ему версию CLT c [офиц.сайт Apple](https://developer.apple.com/download/more/)

Устанавливаем `XCode 8.2.1` из файла `Xcode_8.2.1.xip` и CLT из файла `Command_Line_Tools_macOS_10.11_for_Xcode_8.2.dmg`


## 3. Установка MacPorts и пакетов <a id="3. Установка MacPorts и пакетов"></a>

[Страница со всеми доступными версиями MacPorts](https://www.macports.org/install.php#installing)

[Ссылка на скачивание MacPorts для MacOS ElCapitan](https://github.com/macports/macports-base/releases/download/v2.8.0/MacPorts-2.8.0-10.11-ElCapitan.pkg)

Запускаем файл `.pkg` и следуем инструкциям по установке.

[Страница с доступными Ports](https://ports.macports.org/)

Устанавливаем следующие пакеты:

- *Инструменты для разработки:*
  - `sudo port install git` [details](https://ports.macports.org/port/git/details/)
  - `sudo port install vim` [details](https://ports.macports.org/port/vim/details/)
  - `sudo port install docker` [details](https://ports.macports.org/port/docker/details/)
  - `sudo port install py310-ansible` [details](https://ports.macports.org/port/py310-ansible/details/)
- *Языки программирования:*
  - `sudo port install python310` [details](https://ports.macports.org/port/python310/details/)
  - `sudo port install py310-setuptools` [details](https://ports.macports.org/port/py310-setuptools/details/)
  - `sudo port install nodejs18` [details](https://ports.macports.org/port/nodejs18/details/)
  - `sudo port install php82` [details](https://ports.macports.org/port/php82/details/)
  - `sudo port install ruby31` [details](https://ports.macports.org/port/ruby31/details/)
  - `sudo port install go` [details](https://ports.macports.org/port/go/details/)
- *Базы данных:*
  - `sudo port install sqlite3` [details](https://ports.macports.org/port/sqlite3/details/)
  - `sudo port install mysql57` [details](https://ports.macports.org/port/mysql57/details/)
  - `sudo port install postgresql15` [details](https://ports.macports.org/port/postgresql15/details/)
  - `sudo port install mariadb` [details](https://ports.macports.org/port/mariadb/details/)
  - `sudo port install redis` [details](https://ports.macports.org/port/redis/details/)
- *Web-серверы:*
  - `sudo port install apache2` [details](https://ports.macports.org/port/apache2/details/)
  - `sudo port install nginx` [details](https://ports.macports.org/port/nginx/details/)
- *Среды разработки:*
  - `sudo port install Arduino` [details](https://ports.macports.org/port/Arduino/details/)
- *Инструменты для работы с сетью:*
  - `sudo port install curl` [details](https://ports.macports.org/port/curl/details/)
  - `sudo port install nmap` [details](https://ports.macports.org/port/nmap/details/)
  - `sudo port install wireshark3` [details](https://ports.macports.org/port/wireshark3/details/)
  - `sudo port install elinks` [details](https://ports.macports.org/port/elinks/details/)
- *Инструменты для работы с видео:*
  - `sudo port install youtube-dl` [details](https://ports.macports.org/port/youtube-dl/details/)
  - `sudo port install ffmpeg` [details](https://ports.macports.org/port/ffmpeg/details/)
  - `sudo port install VLC` [details](https://ports.macports.org/port/VLC/details/)
- *Системные утилиты:*
  - `sudo port install htop` [details](https://ports.macports.org/port/htop/details/)
  - `sudo port install neofetch` [details](https://ports.macports.org/port/neofetch/details/)
  - `sudo port install nnn` [details](https://ports.macports.org/port/nnn/details/)
- *Инструменты для работы с графикой:*
  - `sudo port install gimp2` [details](https://ports.macports.org/port/gimp2/details/)
  - `sudo port install ImageMagick` [details](https://ports.macports.org/port/ImageMagick/details/)


## 4. Установка браузеров Chrome и Firefox <a id="4. Установка браузеров Chrome и Firefox"></a>

Доступная версия Google Chrome для MacOS ElCapitan `102.0.5005.63`. Скачиваем с [офиц.сайта Google](https://google-chrome.en.uptodown.com/mac/download/62632406). И устанавливаем из скачанного файла `google-chrome-102-0-5005-63.pkg`.

Доступная версия Firefox для MacOS ElCapitan `78.15.0esr`. Скачиваем с [офиц.сайта Firefox](https://ftp.mozilla.org/pub/firefox/releases/78.15.0esr/mac/ru/) - русская версия, [офиц.сайта Firefox](https://ftp.mozilla.org/pub/firefox/releases/78.15.0esr/mac/en-US/) - английская версия. Устанавливаем из скачанного образа `Firefox 78.15.0esr_ru.dmg` или `Firefox 78.15.0esr_en_US.dmg`

Устанавливаем расширения для Firefox `РуТрекер - официальный плагин (доступ и пр.)`, `AdBlocker Ultimate`, `Print Edit WE`, `SingleFile`, `TWP - Translate Web Pages`


## 5. Установка VirtualBox и виртуальных машин <a id="5. Установка VirtualBox и виртуальных машин"></a>

Доступная версия VirtualBox для MacOS ElCapitan `6.1.40`, скачиваем ее  с [офиц.сайта](https://www.virtualbox.org/wiki/Download_Old_Builds_6_1).

Устанавливаем следующие образы ОС `debian-live-11.5.0-amd64-cinnamon.iso`, `CentOS-7-x86_64-NetInstall-2009.iso`, `kali-linux-2022.3-installer-netinst-amd64.iso`, `ubuntu-22.04.1-live-server-amd64`.

Для виртуальных машин выбираем следующие параметры:

{{< figure src="./2023-01-06-min.jpg" >}}

{{< admonition type=note title="Примечание" open=true >}}
**Для KaliLinux размер жесткого диска необходим 80Гб**
{{< /admonition >}}


## 6. Установка Visual Studio Code <a id="6. Установка Visual Studio Code"></a>

Доступная версия Visual Studio Code для MacOS ElCapitan `1.74.2`, скачиваем ее с [офиц.сайта](https://code.visualstudio.com/Download).

Разархивируем zip-архив и копируем приложение в `Applications`


## 7. Установка MAMP <a id="7. Установка MAMP"></a>

Доступная версия MAMP для MacOS ElCapitan `5.7`, скачиваем ее с [офиц.сайта](https://www.mamp.info/en/downloads/older-versions/), там же есть более старые версии MAMP.
[Ссылка на скачивание версии MAMP 5.7](https://downloads.mamp.info/MAMP-PRO/releases/5.7/MAMP_MAMP_PRO_5.7.pkg)

## 8. Настройка GitHub <a id="8. Настройка GitHub"></a>

```bash
# Generate ssh-key
ssh-keygen -t rsa -b 4096 -C "manin.serg@mail.com"

# Copy public key to clipboard
pbcopy ~/.ssh/id_rsa.pub
```

Добавление нового ключа ssh на GitHub в `Profile/Settings/SSH and GPG keys/New SSH key`. Вставляем скопированный публичный ключ из буфера обмена и даем название.

Тестируем соединение с использованием ssh ключей:

```bash
ssh -T git@github.com
```

Настраиваем `git`:

```bash
git config --global user.name "Sergei Manin"
git config --global user.email "manin.serg@gmail.com"
git config --global github.user maninserg
git config --global color.ui true
```













