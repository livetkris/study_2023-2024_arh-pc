---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Язык разметки Markdown"
author: "Кочкина Кристина Андреевна НММбд-02-23"

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

Целью работы является ознакомление с возможностями разметки Markdown и оформление в ней лабораторную работу №2.

# Задание

Сделать отчет по лабораторной работе №2 в формате Markdown и загрузить на github.

# Теоретическое введение

Базовые сведения о Markdown

Чтобы создать заголовок, используйте знак #, например:

# This is heading 1

## This is heading 2

### This is heading 3

#### This is heading 4

Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:
This text is *italic*.

Оформление формул в Markdown

Внутритекстовые формулы делаются аналогично формулам LaTeX. 

Оформление изображеий в Markdown

В Markdown вставить изображение в документ можно с помощью непосредственного
указания адреса изображения.

Обработка файлов в формате Markdown

Преобразовать файл README.md можно следующим образом:

pandoc README.md -o README.pdf

# Выполнение лабораторной работы
 Открыла терминал.
 
 Перешла в каталог курса (рис.1).
![Перешла в каталог командой cd](image/1.png){#fig:001 width=70%}

Обновила локальный репозиторий (рис.2).
![Обновила репозиторий командой git pull](image/2.png){#fig:002 width=70%}

Перешла в каталог с шаблоном отчёта (рис.3).
![Перешла в каталог report](image/3.png){#fig:003 width=70%}

Проводим компиляцию шаблона (рис.4).
![Используя команду make, создала pdf и docx файлы](image/4.png){#fig:004 width=70%}

Проверила корректность полученных файлов (рис.5).
![Смотрю, появились ли файлы](image/5.png){#fig:005 width=70%}

Удаляю недавно созданные файлы (рис.6).
![Используем команду make clean](image/6.png){#fig:006 width=70%}

Проверяю, удалились ли файлы (рис.7).
![Проверяю, как сработала команда make clean](image/7.png){#fig:007 width=70%}

Открываю файл report.md в текстовом редакторе (рис.8).
![Использую команду gedit](image/8.png){#fig:008 width=70%}

Изучаю данный файл и приступаю к его оформлению для лабораторной работы (рис.9).
![Изучаю файл](image/9.png){#fig:009 width=70%}

# Выводы

Освоила процедуру оформления отчётов с помщью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
