---
## Front matter
title: "Отчет по лабораторной работе №10"
subtitle: "Понятие подпрограммы. Отладчик GDB"
author: "Лушин Артем Андреевич"

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
biblatex: false
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

Приобретение навыков написания программ с использованием подпрограмм.
Знакомство с методами отладки при помощи GDB и его основными возможностями


# Выполнение лабораторной работы

1) Я создал каталог lab10 и создал файл lab10-1.asm

![Создание каталога и файла](image/1.png){ #fig:001 width=70% }

2)Я ввел текст листинга в файл и запустил программу.

![Текст программы](image/2.png){ #fig:002 width=70% }

![Работа программы](image/3.png){ #fig:003 width=70% }

3) Я изменил текст программы, чтобы она решала выражение f(g(x)).

![Измененный текст программы](image/4.png){ #fig:004 width=70% }

![Проверка работы программы](image/5.png){ #fig:005 width=70% }

4)Я создал файл lab10-2.asm и вписал туда программу.

![Текст второй программы](image/6.png){ #fig:006 width=70% }

5)Я загрузил и запустил файл второй программы в отладчик gdb.

![Отладка второго файла](image/7.png){ #fig:007 width=70% }

6) Я поставил брекпоинт на метку _start и запустил программу.

![Брекпоинт на метку _start](image/8.png){ #fig:008 width=70% }

7)Я просмотрел дисассимплированный код программы начиная с метки.

![Дисассимплированный код](image/9.png){ #fig:009 width=70% }

8) С помощью команды я переключился на intel'овское отображение синтаксиса. Отличие заключается в командах, в диссамилированном отображении в командах используют % и $, а в Intel отображение эти символы не используются. На такое отображение удобнее смотреть.

![Intel'овское отображение](image/10.png){ #fig:010 width=70% }

9) Для удобства я включил режим псевдографики.

![Псевдографика](image/11.png){ #fig:011 width=70% }

10) Я посмотрел наличие меток и добавил еще одну метку на предпоследнюю инструкцию.

![Наличие меток](image/12.png){ #fig:012 width=70% }

11) С помощью команды si я посмотрел регистры и изменил их.

![Просмотр регистров](image/13.png){ #fig:013 width=70% }

![Измененные регистры](image/14.png){ #fig:014 width=70% }

12) С помощью команды я посмотрел значение переменной msg1.

![Просмотри значения переменной](image/15.png){ #fig:015 width=70% }

13) Следом я посмотрел значение второй переменной msg2.

![Значение переменной msg2](image/16.png){ #fig:016 width=70% }

14) С помощью команды set я изменил значение переменной msg1.

![Изменение значения переменной](image/17.png){ #fig:017 width=70% }

15)Я изменил переменную msg2.

![Изменение msg2](image/18.png){ #fig:018 width=70% }

16)Я вывел значение регистров ecx и eax.

![Значение регистров ecx и eax](image/19.png){ #fig:019 width=70% }

17) Я изменил значение регистра ebx. Команда выводит два разных значения так как в первый раз мы вносим значение 2, а во второй раз регистр равен двум, поэтому и значения разные.

![Значение регистров ebx](image/20.png){ #fig:020 width=70% }

18) Я завершил работу с файлов вышел.

![Завершение работы с файлов](image/21.png){ #fig:021 width=70% }

19) Я скопировал файл lab9-2.asm и переименовал его. Запустил файл в отладчике и указал аргументы.

![Запуск файла в отладчике](image/22.png){ #fig:022 width=70% }

20) Поставил метку на _start и запустил файл.

![Запуск файла lab10-3 через метку](image/23.png){ #fig:023 width=70% }

21)Я проверил адрес вершины стека и убедился что там хранится 5 элементов.

![Адрес вершины стека](image/24.png){ #fig:024 width=70% }

22) Я посмотрел все позиции стека. По первому адрему хранится адрес, в остальных адресах хранятся элементы. Элементы расположены с интервалом в 4 единицы, так как стек может хранить до 4 байт, и для того чтобы данные сохранялись нормально и без помех, компьютер использует новый стек для новой информации.

![Все позиции стека](image/25.png){ #fig:025 width=70% }

# Самостоятельная работа

1) Я преобразовал программу из лабораторной работы №9 и реализовал вычисления как подпрограмму.

![Текст программы](image/26.png){ #fig:026 width=70% }

![Запуск программы](image/27.png){ #fig:027 width=70% }

2) Я переписал программу и попробовал запустить ее чтобы увидеть ошибку. Ошибка была арифметическая, так как вместо 25,программа выводит 10.

![Текст програмыы](image/28.png){ #fig:028 width=70% }

![Запуск программы](image/29.png){ #fig:029 width=70% }

После появления ошибки, я запустил программу в отладчике.

![Запуск программы в отладчике](image/30.png){ #fig:030 width=70% }

Я открыл регистры и проанализировал их, понял что некоторые регистры стоят не на своих местах и исправил это.

![Анализ регистров](image/31.png){ #fig:031 width=70% }

Я изменил регистры и запустил программу, программа вывела ответ 25, то есть все работает правильно.

![Повторный запуск программы](image/32.png){ #fig:032 width=70% }

# Вывод{.unnumbered}

Я приобрел навыки написания программ использованием подпрограмм. Познакомился с методами отладки при помозь GDB и его основными возможностями.


