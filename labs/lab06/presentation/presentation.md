---
## Front matter
lang: ru-RU
title: Презентация по лабораторной работе №6
subtitle: Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов
author:
  - Плескачева Е.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 17 марта 2023

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

Ознакомиться с инструментами поиска файлов и фильтрации текстовых данных. Приобрести практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

## Задание

• Выполнить все примеры, приведённые в первой части описания лабораторной работы
• Выполните действия, зафиксировав в отчёте по лабораторной работе используемые при этом команды и результаты их выполнения
• Создать отчёт и презентацию в Markdown
• Загрузить скринкасты на видео хостинг
• Представить работу на сайте ТУИС

# Выполнение лабораторной работы

## Шаг 1

![Осуществили вход в систему, используя соответствующее имя пользователя](image/1.png)

## Шаг 2

![Записали в файл file.txt названия файлов, содержащихся в каталоге /etc](image/2.png)

## Шаг 3

![Дописали в этот же файл названия файлов, содержащихся в домашнем каталоге](image/3.png)

## Шаг 4

![С помощью команды cat проверили, что в файле содержатся названия файлов как каталога /etc, так и домашнего каталога](image/4.png)

## Шаг 5

![Вывели имена всех файлов из file.txt, имеющих расширение .conf](image/5.png)

## Шаг 6

![Записали их в новый текстовой файл conf.txt](image/6.png)

## Шаг 7

![Определили, какие файлы в домашнем каталоге имеют имена, начинающиеся с символа c](image/7.png)

## Шаг 8

![Вывели на экран имена файлов из каталога /etc, начинающиеся с символа h](image/8.png)

## Шаг 9

![Запустили в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log](image/9.png)

## Шаг 10

![С помощью команды jobs проверили, что процесс работает в фоновом режиме](image/10.png)

## Шаг 11

![С помощью команды cat проверили, что в файле содержатся названия файлов, начинающихся на log](image/11.png)

## Шаг 12

![Проверили, что созданный файл logfile находится в домашнем каталоге](image/12.png)

## Шаг 13

![После удаления файла ~/logfile с помощью команды jobs увидели, что процесс всё ещё запущен](image/13.png)

## Шаг 14

![Запустили из консоли в фоновом режиме редактор gedit](image/14.png)

## Шаг 15

![Прочли справку (man) команды kill](image/15.png)

## Шаг 16

![Завершили процесс с помощью команды kill, посылая сигнал SIGKILL, имеющий номер 9, процессу 4148](image/16.png)

## Шаг 17

![Получили подробную информацию о команде df с помощью команды man](image/17.png)

## Шаг 18

![Получили подробную информацию о команде du с помощью команды man](image/18.png)

## Шаг 19

![ Выполнили команду df](image/19.png)

## Шаг 20

![Выполнили команду du](image/20.png)

## Шаг 21

![Воспользовавшись справкой команды find, вывели имена всех директорий, имеющихся в домашнем каталоге](image/21.png)

# Результаты работы

  С помощью type d мы попросили команду find искать только каталоги. С помощью maxdepth 1 мы попросили команду find сохранить поиск только на текущем уровне (и не заходить в подкаталоги). Введёная команда также показывает скрытые каталоги.

## Выводы

 Ознакомились с инструментами поиска файлов и фильтрации текстовых данных. Приобрели практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.


