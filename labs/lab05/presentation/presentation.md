---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе №5
subtitle: Анализ файловой системы Linux. Команды для работы с файлами и каталогами
author:
  - Плескачева Е.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 10 марта 2023

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Плескачева Елизавета Андреевна
  * учебная группа: НММбд-02-22
  * студент направления Математика и Механика
  * Российский университет дружбы народов
  * [1132226461@pfur.ru](mailto:1132226461@pfur.ru)
  * <https://github.com/kukusb>

:::
::: {.column width="30%"}

![](./image/me.jpg)

:::
::::::::::::::

# Вводная часть

## Цель работы

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

## Задание

Повторить команды-примеры. Выполнить задания для самостоятельной работы для приобретения навыков применения команд системы Linux.

# Выполнение лабораторной работы

## Шаг 1

![Скопировали файл ~/abc1 в файл april и в файл may](image/1.png)

## Шаг 2

![Скопировали файлы april и may в каталог monthly](image/2.png)

## Шаг 3

![Скопировали файл monthly/may в файл с именем june](image/3.png)

## Шаг 4

![Скопировали каталог monthly в каталог monthly.00 и каталог monthly.00 в каталог /tmp](image/4.png)

## Шаг 5

![Изменить название файла april на july в домашнем каталоге](image/5.png)

## Шаг 6

![Переместили файл july в каталог monthly.00](image/6.png)

## Шаг 7

![Переименовать каталог monthly.00 в monthly.01,переместили каталог monthly.01в каталог reports](image/7.png)

## Шаг 8

![Переименовать каталог reports/monthly.01 в reports/monthly](image/8.png)

## Шаг 9

![Создали файл ~/may с правом выполнения для владельца](image/9.png)

## Шаг 10

![Лишили владельца файла ~/may права на выполнение](image/10.png)

## Шаг 11

![Создали каталог monthly с запретом на чтение для членов группы и всех остальных пользователей](image/11.png)

## Шаг 12

![Создали файл ~/abc1 с правом записи для членов группы](image/12.png)

## Шаг 13

![Скопировали файл /usr/include/sys/io.h в домашний каталог и назвали его equipment](image/13.png)

## Шаг 14

![В домашнем каталоге создали директорию ~/ski.plases](image/14.png)

## Шаг 15

![Переместили файл equipment в каталог ~/ski.plases](image/15.png)

## Шаг 16

![Переименовали файл ~/ski.plases/equipment в ~/ski.plases/equiplist](image/16.png)

## Шаг 17

![Создали в домашнем каталоге файл abc1 и скопировали его в каталог ~/ski.plases, назвали его equiplist2](image/17.png)

## Шаг 18

![Создали каталог с именем equipment в каталоге ~/ski.plases и переместили файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment](image/18.png)

## Шаг 19

![Создали и переместили каталог ~/newdir в каталог ~/ski.plases и назвали его plans](image/19.png)

## Шаг 20

Определение опции команды chmod

 1. australia (a+r u+w u+x)
 2. play (a+x u+r u+w)
 3. my_os (a+r u+x)
 4. feathers (a+r a+w o-w)
 
## Шаг 21 

Выполнение упражнений 

 1. Просмотрели содержимое файла с помощью команды ls /etc/password
 2. Скопировали файл ~/feathers в файл ~/file.old с помощью команды cp ~/feathers ~/file.old
 3. Переместили файл ~/file.old в каталог ~/play с помощью команды mv file.old ~/play
 4. Скопировали каталог ~/play в каталог ~/fun с помощью команды cp
 5. Переместили каталог ~/fun в каталог ~/play и назовите его games с помощью команды mv ~/fun ~/play/games
 6. Лишили владельца файла ~/feathers права на чтение с помощью команды chmod u-r
 7. Если просмотреть файл ~/feathers командой cat, то выдаётся ошибка “Отказано в доступе”
 8. Скопировать файл feathers не удаётся по той же ошибке
 9. Дали владельцу файла ~/feathers право на чтение с помощью команды
chmod u+r
 10. Лишили владельца каталога ~/play права на выполнение с помощью команды chmod u-x
 11. После выполнения команды перейти в каталог play не представляется возможным
 12. Дали владельцу каталога ~/play право на выполнение с помощью команды chmod u+x

# Результаты работы

## Выводы

Ознакомились с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобрели практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы


