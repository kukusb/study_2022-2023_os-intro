---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
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

 Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

Ознакомиться с форматами команд cd,ls,pwd,mkdir и другими. Выполнить список заданий на отработку этих команд

# Выполнение лабораторной работы

![Определили полное имя домашнего каталога](image/1.png)

![Перешли в каталог /tmp](image/2.png)

![Вывели на экран содержимое каталога /tmp c помощью команды ls](image/3.png)

![Применили команду ls с опцией -a, с ее помощью вывели скрытые каталоги](image/4.png)

![Применили команду ls с опцией -l, с ее помощью вывели подробную информацию о файлах и каталгах](image/5.png)

![Выяснили, что в каталоге /var/spool есть подкаталог с именем cron](image/6.png)

![Перешли в домашний каталог с помощью команды cd и вывели на экран его содержимое](image/7.png)

![С помощью команды ls -l определили, что мы являемся владельцем файлов и каталогов](image/8.png)

![В домашнем каталоге создали новый каталог с именем newdir и проверили, что он создался](image/9.png)

![В этом каталоге создали новый катлог с именем morefun](image/10.png)

![В домашнем каталоге одной командой создали три каталга: letters,memos,misk и проверили их создание](image/11.png)

![Затем удалили эти каталоги одной командой, проверили, что каталоги удалились](image/12.png)

![Попытались удалить созданный каталог /newdir командой rm, не получилось, так как для удаления каталога нужно добавить dir к команде rm, затем удалили подкаталог morefun каталога newdir](image/13.png)

![C помощью команды man определили, что опция -R команды ls позволяет просмотреть содержимое не только указанного каталога, но и его подкаталогов](image/14.png)

![C помощью команды man определили, что опция -c команды ls позволяет отсортирвать по времени последнего изменения выводимый список содержимого каталога ](image/15.png)

![Использовали команду man для просмотра описания команды cd. данная команда перемещает пользователя по рабочей директории](image/16.png)

![Использовали команду man для просмотра описания команды pwd. Данная команда выводит на экран все файлы той рабочей директории, в которой пользователь находится](image/17.png)

![Использовали команду man для просмотра описания команды mkdir. Данная команда создает новый каталог в указанном месте или по умолчанию в той рабочей директории, в которой находится пользователь](image/18.png)

![Использовали команду man для просмотра описания команды rmdir. Данная команда удаляет каталог, если в нем нет других файлов или подкаталогов](image/19.png)

![Использовали команду man для просмотра описания команды rm. Данная команда удаляет файлы и каталоги ](image/20.png)

![После вывода списка истории команд с помощью команды history выполнили модификацию команды man и исполнили новую](image/21.png)

![Сделали то же самое с другой командой](image/22.png)


# Выводы

 Выполнили поставленный задачи с отработкой выученных команд. Приобрели практическе навыки взаимодействия пользователя с системой посредством командной строки.


