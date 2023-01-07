
---
title: "Чистая установка MacOS ElCapitan"
date: 2023-01-05T22:04:28+03:00
draft: false
author: "Segei Manin"
tags: ["MacOS", "configuration"]
categories: [Configuration]
slug: “clean-install-macos-elcapitan”
---


## 1. Скачиваем установщик MacOS ElCapitan  <a id="1. Скачиваем установщик MacOS ElCapitan "></a>

[Страница сo всеми доступными версиями MacOS на офиц.сайте](https://support.apple.com/ru-ru/HT211683)

[Ссылка загрузки MacOS ElCapitan 10.11.6](https://support.apple.com/ru-ru/HT211683)


## 2. Установка установщика MacOS ElCapitan <a id="2. Установка установщика MacOS ElCapitan"></a>

Дважды щелкаем на скаченный файл `.dmg`. Дважды щелкаем на файл `.pkg`. Следуем инструкциям. Установщик MacOS ElCapitan будет установлен в папку `Applications`.


## 3. Создание загружаемого установщика на флеш-накопителе USB или встроенном томе<a id="3. Создание загружаемого установщика на флеш-накопителе USB или встроенном томе"></a>

Флеш-накопитель USB или другой том должен иметь емкомсть не менее 14 Гб и быть отформатированным с файловой системой `MacOS Extended (Journaled)`.

{{< admonition type=tip title="Совет" open=true >}}
*Вместо флеш-накопителя USB более оптимальным является использовать специально выделенный том в конце встроенного жесткого диска компьютера, если в дальнейшем требуется установка только на этот компьютер.*
{{< /admonition >}}


Открываем приложение `Terminal`. И вставляем команду:

```bash
sudo /Applications/Install\ OS\ X\ El\ Capitan.app/Contents/Resources/createinstallmedia 
--volume /Volumes/MyVolume --applicationpath /Applications/Install\ OS\ X\ El\ Capitan.app
```
Где **`/Volumes/MyVolume`** обозначает путь монтирования флеш-накопителя USB или другого используемого тома. Берется из `Disk Utility`.


## 4. Чистая установка MacOS ElCapitan<a id="4. Чистая установка MacOS ElCapitan"></a>

Включить компьтер, зажав клавиши  `⌘ Cmd` и `R` во время загрузки. В загрузившемся приложении `Utilites OS X` выбрать пункт `Disk Utility` и отформатировать диск для установки системы в файловой системе `MacOS Extended (Journaled)`.

Завершить приложение `Utilities OS X` с помощью меню `Utilites OS X / Finish Utilites OS X`. В появившемся меню нажать `Boot disk...`, выбрать USB флеш-накопитель с установщиком MacOS ElCapitan и нажать `Reboot...`.

Запустить MacOS установщик можно и при перезгрузке, зажав клавишу `⌥Option (Alt)` и выбрав USB флеш-накопитель в появившемся меню.
