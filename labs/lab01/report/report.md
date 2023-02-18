---
## Front matter
title: "Отчет по лабораторной работе №1"
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
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

Приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задания

Создать виртуальную машину, установить операционную систему,выполнить все требуемые настройки и установить требуемые программы

# Выполнение лабораторной работы

## Настройка каталога для виртуальных машин

![Запустили терминал и перешли в каталог /var/tmp](image/1.png)

![Создали каталог с именем пользователя с помощью команды mkdir /var/tmp/`id -un`](image/2.png)

## Создание виртуальной машины

![Запустили менеджер виртуальных машин с помощью команды VirtualBox &](image/3.png)

![Установили папку для виртуальных машин в /var/tmp/имя_пользователя](image/4.png)

![Настроили хост-клавишу, чтобы избежать конфликта значений с переключателем языка ввода](image/5.png)

![Задали имя и образ операционной системы виртуальной машины](image/6.png)

![Задали размер основной памяти виртуальной машины](image/7.png)

![Задали контроллеры](image/8.png)

![Установили настройки дисплея ](image/9.png)

## Установка системы на диск

![Установили русский язык интерфейса в настройках Fedora](image/10.png)

![Задали конфигурацию жесткого диска ](image/11.png)

![Установили имя и пароль для пользователя root](image/12.png)

![Установили имя узла](image/13.png)

![Установили имя и пароль для нашего пользователя](image/14.png)

![Убедились в правильности заданных настроек](image/15.png)

![Дождались завершения установки операционной системы, после чего корректно перезапустили виртуальную машину](image/16.png)

## Действия после установки 

![Запустили терминал с помощью комбинации клавиш Win+Enter и переключились на роль супер-пользователя с помощью команды sudo -i](image/17.png)

![Обновили все пакеты с помощью команды dnf -y update](image/18.png)

![Использовали команду dnf install tmux mc для удобства работы в консоли](image/19.png)

![Установили программное обеспечение с помощью команды dnf install dnf-automatic](image/20.png)

![Запустили таймер](image/21.png)

![В файле /etc/selinux/config заменили значение SELINUX=enforcing на значение SELINUX=permissive, затем перезагрузили виртуальную машину с помощью команды reboot](image/22.png)

## Установка драйверов для VirtualBox

![Запустили терминальный мультиплексор и преключились на роль супер-пользователя](image/23.png)

![Установили пакет DKMS с помощью команды dnf -y install dkms](image/24.png)

![Подмонтировали диск ](image/25.png)

#Домашнее задание
Получили следующую информацию:

![Версия ядра Linux (Linux version)](image/26.png)

![Частота процессора (Detected Mhz processor)](image/27.png)

![Модель процессора (CPU0)](image/28.png)

![Объём доступной оперативной памяти (Memory available)](image/29.png)

![Тип обнаруженного гипервизора (Hypervisor detected)](image/30.png)

![Тип файловой системы корневого раздела.](image/31.png)

![Последовательность монтирования файловых систем](image/32.png)

# Контрольные вопросы

1. Какую информацию содержит учетная запись пользователя?
Имя пользователя (user name)
Индентификационный номер пользвателя (UID)
Индентификационный номер группы (GID)
Пароль (password)
Полное имя (full name)
Домашний каталог (home directory)
Начальную оболочку (login shell)

2. Укажите команды терминала и приведите примеры:

    для получения справки по команд
    -help
    для перемещения по файловой системе
    -cd
    для просмотра содержимого каталога
    -ls
    для определения объёма каталога
    -du
    для создания / удаления каталогов / файлов
    -mkdir / rm -r 
    для задания определённых прав на файл / каталог
    -touch/rm
    для просмотра истории команд
    -history

3. Что такое файловая система? Приведите примеры с краткой характеристикой
 Файловая система - порядок, определяющий способ организациии, хранения и наименования данных на носителях в пк, а также в другом электронном оборудовании: мобильных телефонах или цифровых фотоаппаратах. Она так же определяет формат содержимого и способ физического хранения информации. Некоторые могут представлять сервисные возможности, например, разграничение доступа
 
 4. Как посмотреть, какие файловые системы подмонтированы в ОС?
 Df - утилита, которая показывает список всех файловых систем по имени устройства, сообщает их размер, занятое и свободное пространство и точки монтировния. 
 
 5. Как удалить зависший процесс?
 
с помощью команды killall-killall().

# Выводы

Приобрели практические навыки установки операционной системы на виртуальную машину и настройки необходимых для дальнейшей работы сервисов.


