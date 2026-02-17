---
## Front matter
title: "Отчёт по лабораторной работе 1"
subtitle: "Установка и конфигурация ОС на виртуальную машину"
author: "Серебрякова Дарья Ильинична"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Выполнение лабораторной работы

## Создание и настройка виртуальной машины

Установила Rocky Linux и задала необходимые параметры в виде памяти, количества ядер и тд. Запустила виртуальную машину и выбрала язык интерфейса (рис. 1).

![Выбор языка интерфейса](image/1.JPG){#fig:001 width=70%}

Добавляю русскую раскадку и устанавливаю клавиши для переключения (рис. 2).

![Добавление русской раскладки](image/2.JPG){#fig:002 width=70%}

В разделе выбора программ указала в качестве базового окружения Server with GUI , а в качестве дополнения — Development Tools (рис. 3).

![Выбор окружения](image/3.JPG){#fig:003 width=70%}

Отключфю KDUMP (рис. 4).

![KDUMP](image/4.JPG){#fig:004 width=70%}

## Создание учетной записи и пользователя

Задаю имя пользователя (рис. 5).

![Имя пользователя](image/5.JPG){#fig:005 width=70%}

Задаю пользователя с правами администратора и устанавливаю пароль (рис. 6).

![Установка пароля](image/6.JPG){#fig:006 width=70%}

Перезапускаю виртуальную машину и вхожу в свою учетную запись (рис. 7).

![Вход в ОС](image/7.JPG){#fig:007 width=70%}

Установила имя пользователя и имя хоста (рис. 8).

![Имя пользователя](image/8.JPG){#fig:008 width=70%}

# Контрольные вопросы

1) Какую информацию содержит учетная запись пользователя?

Имя пользователя, зашифрованный пароль пользователя, индентификационный номер пользователя, индентификационный номер группы пользователя, домашний каталог пользователя, командный интерпретатор пользователя.

2) Укажите команды терминала и приведите примеры: 
-для получения справки по команде: man <назввание команды> man cd
-ддя перемещения по файловой системе: cd cd ~/Downloads
-для просмотра содержимого каталога: ls ls ~/Downloads
-для определения объема каталога: du <имя каталога> du Downloads
-для создания каталогов: mkdir <имя каталога> mkdir ~/Downloads/New
-для создания файлов: touch <имя файла> touch retouch
-для удаления каталогов: rm <имя каталога> rm dir1
-для удаления файлов: rm -r <имя файла> rm -r text.txt
-для задания определенных прав на файл или каталог: chmod + x <имя каталога или файла> chmod +x text.txt
-для просмотра истории команд: history

3) Что такое файловая система? Приведите примеры с краткой характеристикой.

Файловая система - это часть операционной системы, назначение которой состоит в том, чтобы обеспечить пользователю удобный интерфейс при работе с данными, хранящимися на диске, и обеспечить совместное использование файлов несколькими пользователями и процессорами.
Примеры файловых систем: 
Ext2, Ext3, Ext4 или Extended Felisystem - стандартная файловая система для Linux.
NTFS (New Technology File System):  Стандартная файловая система для Windows.

4) Как посмотреть, какие файловые системы подмонтированы в ОС?

С помощью команды mount

5) Как удалить зависший процесс?

С помощью команды kill.

# Выводы

В результате выполнения лабораторной работы мы приобрели навыки установки операционной системы на виртуальную машину, а также настройки минимально необходимых для дальнейшей работы сервисов.









