---
## Front matter
title: "Отчёт по лабораторной работе 4"
subtitle: "Архитектура компьютера"
author: "Гуламова Е.М. НПИбд-03-23"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
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

Целью работы является освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Выполнение лабораторной работы

1. Я создала папку lab04, используя команду mkdir, затем перешла в неё с помощью команды cd и создала файл hello.asm.

![Создание каталога и файла](image/01.png){ #fig:001 width=70%, height=70% }

2. Открыла файл и составила код программы, следуя заданию.

![Программа в файле hello.asm](image/02.png){ #fig:002 width=70%, height=70% }

3. Произвела трансляцию файла с помощью nasm и получила объектный файл hello.o.

4. Запустила трансляцию файла с помощью nasm, используя дополнительные параметры, и в результате создала файл листинга list.lst, объектный файл obj.o, а в программу была добавлена отладочная информация.

5. Провела линковку с помощью команды ld, в результате чего получила исполняемый файл.

6. Повторила процесс линковки для объектного файла obj.o и создала исполняемый файл main.

7. Запустила исполняемые файлы.

![Трансляция, линковка и запуск программы](image/03.png){ #fig:003 width=70%, height=70% }

8. Изменила текст выводимого сообщения с "Hello world" на своё имя и запустила файл снова.

![Программа в файле lab4.asm](image/04.png){ #fig:004 width=70%, height=70% }

![Сборка и проверка программы lab4.asm](image/05.png){ #fig:005 width=70%, height=70% }

# Выводы

Освоили процесс компиляции и сборки программ, написанных на ассемблере nasm.