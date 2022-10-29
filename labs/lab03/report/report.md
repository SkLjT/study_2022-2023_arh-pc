---
## Front matter
title: "ЛАБОРАТОРНАЯРАБОТА № 3"
subtitle: "Система контроля версий Git"
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
fontsize: 13pt
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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Изучить идеологию и применение средств контроля версии. Приобрести навыки по работе с системой git.



# Выполнение лабораторной работы

1.1) Я создал аккаунт на сайте GitHub

![Создание аккаунта githun](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032201.jpeg){ #fig:001 width=70% }

![Профиль на github](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032209.jpeg){ #fig:002 width=70% }

1.2) Я сделал предварительную конфигурацию с помощью введеных команд.

![Предварительная кофигурация.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032216.jpeg){ #fig:003 width=70% }

1.3) Я создал SSH – ключ. 

![Генерация приватного  и открытого ключа.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032222.jpeg){ #fig:004 width=70% }

![Вывел ключ из консоль для переноса на сайт](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032231.jpeg){ #fig:005 width=70% }

![Зарегистрировал ключ на сайте и сохранил его.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032237.jpeg){ #fig:006 width=70% }

1.4) Я создал каталог для предмета “Архитектура компьютера”

![Создание каталога.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032243.jpeg){ #fig:007 width=70% }

1.5) Я создал репозиторий на сайте.

![Репозиторий на сайте.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032248.jpeg){ #fig:008 width=70% }

1.6)Я клонировал созданный репозиторий через консоль. 

![Репозиторий через консоль.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032253.jpeg){ #fig:009 width=70% }

1.7)Я удалил лишние файлы из каталога курса, создал новые и отправил на сервер.

![Удаление лишних файлов и создание новых.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032258.jpeg){ #fig:010 width=70% }

![Отправка новых файлов на сервер.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032264.jpeg){ #fig:011 width=70% }

1.8) Я проверил правильность создания иерархии на странице github.

![Проверка иерархии на github](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667032270.jpeg){ #fig:012 width=70% }



# Выполнение самостоятельной работы.

3.1. Я создал отчет по лабораторной работе и перенес его в гостевую операционную систему.  Затем через команды перенес в папку Lab03. 

![Перенес папку в соответствующий каталог.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034042.jpeg){ #fig:013 width=70% }

3.1’. Перенес файл на github с помощью команд add и push.

![Перенес файлы на сайт github.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034046.jpeg){ #fig:014 width=70% }

3.1”. Я проверил правильность переноса данных на сайте.

![Проверка задания на сайте.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034051.jpeg){ #fig:015 width=70% }

3.2. Я перенес файлы первой и второй лабораторной работы в домашнюю директорию linux.

![Файлы двух лабораторных.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034055.jpeg){ #fig:016 width=70% }

3.2’. Я перенес файлы в соответствующие каталоги.

![Перенос файлов в каталоге.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034058.jpeg){ #fig:017 width=70% }

3.2”. С помощью команд перенес все внесенные данные на сайт.

![Перенос данных на сайт.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034062.jpeg){ #fig:018 width=70% }

3.2’’’. Проверил все ли перенеслось. 

![Проверил данные на сайте github.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab03/report/image/photo1667034065.jpeg){ #fig:019 width=70% }



# Вывод

Я изучил идеологию и применение средств контроля. Овладел системой github.


::: {#refs}
:::
