---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Первоначальная настройка git"
author: "Плескачева Елизавета Андреевна НММ-02-22бд"

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

Изучить идеологию и применение средств контроля версий и освоить умения по работе с git

# Задание

Установить git, выполнить базовую настройку, создать ключ, создать репозиторий курса и настроить его

# Выполнение лабораторной работы

git уже был установлен на пк в дисплейном классе, поэтому загрузили его на виртуальную машину

![загрузили git](image/1.png)

![Задали имя и почту владельца репозитория](image/3.png)

![Настроили utf-8 в выводе сообщение git](image/4.png)

![Задали имя начальной ветки](image/5.png)

![Выполнили параметры autocrlf и safecrlf](image/6.png)

ssh ключ уже был создан нами во время выполнения лабораторной работы в прошлом семестре, для удобства будем использовать его

![По образцу создали каталог курса](image/7.png)

![удалили ненужные файлы и создали необходимые каталоги](image/8.png)

![отправили файлы на сервер](image/9.png)

# Выводы
Научились работать с git, изучили идеологию и контроль над версиями.

