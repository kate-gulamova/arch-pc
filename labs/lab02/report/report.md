---
## Front matter
title: "Отчёт по лабораторной работе 2"
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

Изучить идеологию и научиться применять средства контроля версий. Получить практические навыки по работе с системой git.
  
# Ход работы

Чтобы начать работать с GitHub (далее — гитхаб) нужно зарегистрироваться

![Данные для регистрации аккаунта на Гитхабе](image/01.png){ #fig:001 width=70%, height=70% }

Далее я нахожу на Гитхабе шаблонный репозиторий и создаю свой

![Создание своего репозитория на основании шаблона](image/02.png){ #fig:002 width=70%, height=70% }

![ Создание репозитория](image/03.png){ #fig:003 width=70%, height=70% }

Делаю предварительную настройку git

![Выполнение команд для предварительной настройки Гитхаб](image/04.png){ #fig:004 width=70%, height=70% }

Для последующей работы необходимо сгенерировать пару ключей идентификации

![Выполнение команд для создания SSH ключа](image/05.png){ #fig:005 width=70%, height=70% }

Теперь необходимо добавить свой ключ на Гитхаб по названием  «Title»

![Добавление своего ключа на Гитхаб](image/06.png){ #fig:006 width=70%, height=70% }

Далее необходимо создать рабочий каталог

![Создание рабочего каталога](image/07.png){ #fig:007 width=70%, height=70% }

Теперь я создаю курс

![Создание курса](image/08.png){ #fig:008 width=70%, height=70% }

Далее нужно отправить эти данные на Гитхаб

![Отправка данных на Гитхаб ч.1](image/09.png){ #fig:009 width=70%, height=70% }

![Отправка данных на Гитхаб ч.2](image/10.png){ #fig:010 width=70%, height=70% }

![Результат проделанной работы](image/11.png){ #fig:011 width=70%, height=70% }

# Выводы

Я получил навыки по работе с системой контроля версий GitHub.