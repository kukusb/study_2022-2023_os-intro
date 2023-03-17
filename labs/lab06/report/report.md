---
## Front matter
title: "Отчёт по лабораторной работе №6"
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
author: "Плескачева Елизавета Андреевна"

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

   Ознакомиться с инструментами поиска файлов и фильтрации текстовых данных. Приобрести практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Задание

• Выполнить все примеры, приведённые в первой части описания лабораторной работы
• Выполните действия, зафиксировав в отчёте по лабораторной работе используемые при этом команды и результаты их выполнения
• Создать отчёт и презентацию в Markdown
• Загрузить скринкасты на видео хостинг
• Представить работу на сайте ТУИС

# Выполнение лабораторной работы

![Осуществили вход в систему, используя соответствующее имя пользователя](image/1.png)

![Записали в файл file.txt названия файлов, содержащихся в каталоге /etc](image/2.png)

![Дописали в этот же файл названия файлов, содержащихся в домашнем каталоге](image/3.png)

![С помощью команды cat проверили, что в файле содержатся названия файлов как каталога /etc, так и домашнего каталога](image/4.png)

![Вывели имена всех файлов из file.txt, имеющих расширение .conf](image/5.png)

![Записали их в новый текстовой файл conf.txt](image/6.png)

![Определили, какие файлы в домашнем каталоге имеют имена, начинающиеся с символа c](image/7.png)

![Вывели на экран имена файлов из каталога /etc, начинающиеся с символа h](image/8.png)

![Запустили в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log](image/9.png)

![С помощью команды jobs проверили, что процесс работает в фоновом режиме](image/10.png)

![ С помощью команды cat проверили, что в файле содержатся названия файлов, начинающихся на log](image/11.png)

![Проверили, что созданный файл logfile находится в домашнем каталоге](image/12.png)

![После удаления файла ~/logfile с помощью команды jobs увидели, что процесс всё ещё запущен](image/13.png)

![Запустили из консоли в фоновом режиме редактор gedit](image/14.png)

![Прочли справку (man) команды kill](image/15.png)

![Завершили процесс с помощью команды kill, посылая сигнал SIGKILL, имеющий номер 9, процессу 4148](image/16.png)

![Получили подробную информацию о команде df с помощью команды man](image/17.png)

![Получили подробную информацию о команде du с помощью команды man](image/18.png)

![ Выполнили команду df](image/19.png)

![Выполнили команду du](image/20.png)

![Воспользовавшись справкой команды find, вывели имена всех директорий, имеющихся в домашнем каталоге](image/21.png)

  С помощью type d мы попросили команду find искать только каталоги. С помощью maxdepth 1 мы попросили команду find сохранить поиск только на текущем уровне (и не заходить в подкаталоги). Введёная команда также показывает скрытые каталоги.

# Выводы

   Ознакомились с инструментами поиска файлов и фильтрации текстовых данных. Приобрели практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.


