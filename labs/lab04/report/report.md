---
## Front matter
title: "Отчёта по лабораторной работе №4"
subtitle: "Создание и процесс обработки программ на языке ассемблера NASM"
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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить процедуры компиляции, познакомиться с языком ассемблера NASM.

# Задание

Написать 2 программы(Hello world и lab4(Имя Фамилия))

# Выполнение лабораторной работы

## Программа Hello world!

Создаем каталог для работы с программами на языке ассемблера NASM (рис. @fig:001).

![Создаем каталоги с помощью команды mkdir](image/1.jpg){#fig:001 width=70%}

Переходим в  созданный каталог (рис. @fig:002).

![Переходим в каталог с помощью команды сd](image/2.jpg){#fig:002 width=70%}

Создаем текстовый файл (рис. @fig:003).

![Создаем текстовый файл hello.asm и проверяем, создался ли он](image/3.jpg){#fig:003 width=70%}

Открываем данный файл в текстовом редакторе (рис. @fig:004).

![Открываем файл](image/4.jpg){#fig:004 width=70%}

![Заполняем файл по примеру](image/5.jpg){#fig:005 width=70%}

## Транаслятор NASM

Преобразуем текст программы в объектный код (рис. @fig:006).

![Используем команду nasm и проверяем его работу](image/6.jpg){#fig:006 width=70%}

## Расширенный синтаксис командной строки NASM

Компилируем исходный файл (рис. @fig:007).

![Преобразуем файл hello.asm в obj.o и проверяем файлы](image/7.jpg){#fig:007 width=70%}

## Компоновщик LD

Передаем объектный файл на обработку компоновщику (рис. @fig:008).

![Используем команду ld и проверяем создался ли исполняемый файл](image/8.jpg){#fig:008 width=70%}

Передаем объектный файл на обработку компоновщику (рис. @fig:009).

![Используем команду ld, создавая файл main](image/9.jpg){#fig:009 width=70%}

## Запуск исполняемого файла

Запускаем на выполнение созданный исполняемый файл (рис. @fig:010).

![Используем команду ./hello](image/10.jpg){#fig:010 width=70%}

## Задание для самостоятельной работы

Создаем копию файла hello.asm (рис. @fig:011).

![Используем команду cp](image/11.jpg){#fig:011 width=70%}

Открываем файл и редактируем его (рис. @fig:012).

![Редактируем файл для своего имени и фамилии](image/12.jpg){#fig:012 width=70%}

Прописывем те же команды, что и с первой программой.

Запускаем команду (рис. @fig:013).

![Запускаем программу и проверяем вывод](image/13.jpg){#fig:013 width=70%}

Копируем файлы в локальный репозиторий (рис. @fig:014).

![Копируем файлы в каталог с 4 Лабораторной работой](image/14.jpg){#fig:014 width=70%}

Переходим в каталог лабораторных работ и загружаем файлы на Github.

# Выводы

Мы познакомились с языком ассемблера NASM и создали две работающих программы.
