---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Язык разметки Markdown"
author: "Лушин Артем Андреевич"

## Generic otions
lang: ru-RU

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

Овладеть практическими навыками легковесного языка разметки Markdown.


# Выполнение лабораторной работы

1. Я обновил локальный репозиторий скачав изменения из удаленного репозитория. 

![Обновление репозитория.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996671.jpeg){ #fig:001 width=70% }

1.2. Я проверил команду make, она создала два файла report.docx и report.pdf

![Команда make.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996676.jpeg){ #fig:002 width=70% }

1.3. C помощью команды make clean я отчистил созданные файлы и проверил это.

![Команда make clean.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996684.jpeg){ #fig:003 width=70% }

![Проверка отчистки файлов.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996688.jpeg){ #fig:004 width=70% }

1.4. С помощью текстового редактора gedit открыл файл report.md.

![Команда gedit](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996692.jpeg){ #fig:005 width=70% }

![Report.md с помощью gedit.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666996697.jpeg){ #fig:006 width=70% }

1.5. Я заполнил отчет в файле report.md.

![Пункты в файле report.md](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666999413.jpeg){ #fig:007 width=70% }

![Скриншоты выполнения лабораторной работы в каталоге image.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1666999415.jpeg){ #fig:008 width=70% }

1.6. Я перенес файлы на github.

![Перенос файлов на github.](/home/aalushin/work/study/2022-2023/Архитектура компьютера/study_2022-2023_arh-pc/labs/lab04/report/image/photo1667000917.jpeg){ #fig:009 width=70% }


# Выводы

Я овладел практическими навыками легковесного языка разметки Markdown.


