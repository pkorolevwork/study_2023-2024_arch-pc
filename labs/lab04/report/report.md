---
## Front matter
title: "Отчет по лабораторной работе 4"

author: "Королев Павел Алексеевич"

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

Освоение процедуры компиляции и сборки программ на языке ассемблера NASM.

# Задание

1. Написать программу "Hello World" на языке NASM
2. Оттранслировать исходный код в объектный файл
3. Скомпоновать объектный код в исполняемый
4. Запустить исполняемый код


# Теоретическое введение

Ассемблер NASM предназначен для программирования на низкоуровневом языке, максимально приближенном к аппаратному уровню. Программы на ассемблере выполняются значительно быстрее, чем на языках высокого уровня.


# Выполнение лабораторной работы

Перемещаюсь в директорию lab4 (рис. 1).

![рис. 1](image/01.jpg){#fig:001 width=70%}

Создаю пустой файл формата NASM с помощью команды touch (рис. 2).

![рис. 2](image/02.jpg){#fig:001 width=70%}

Открываю файл hello.asm c помощью mousepad (рис. 3).

![рис. 3](image/03.jpg){#fig:001 width=70%}

Пишу необходимый код для вывода "Hello world!" (рис. 4).

![рис. 4](image/04.jpg){#fig:001 width=70%}

Оттранслирую код в объектный файл (рис. 5).

![рис. 5](image/05.jpg){#fig:001 width=70%}

Получаю из транслятора объектный файл и файл листинга (рис. 6).

![рис. 6](image/06.jpg){#fig:001 width=70%}

Просматриваю содержимое директории с помощью команды ls (рис. 7).

![рис. 7](image/07.jpg){#fig:001 width=70%}

Создаю и просматриваю в директории исполняемые файлы hello и main (рис. 8).

![рис. 8](image/08.jpg){#fig:001 width=70%}

Исполняю полученную программу c успешным результатом (рис. 9).

![рис. 9](image/09.jpg){#fig:001 width=70%}

# Выполнение задания для самостоятельной работы

Копирую файл hello.asm в созданный файл lab 4.asm(рис. 10).

![рис. 10](image/10.jpg){#fig:001 width=70%}

Изменяю выводымый программой текст в коде (рис. 11).

![рис. 11](image/11.jpg){#fig:001 width=70%}

 Оттранслирую код в объектный файл (рис. 12).

![рис. 12](image/12.jpg){#fig:001 width=70%}

Преобразую lab4.o в исполняемый файл (рис. 13).

![рис. 13](image/13.jpg){#fig:001 width=70%}

Исполняю полученную программу c успешным результатом (рис. 14).

![рис. 14](image/14.jpg){#fig:001 width=70%}

Создаю необходимую директорию и копирую в нее содержимое work/study/2023-2024/Computer architecture/arch-pc/labs/lab04 (рис. 15).

![рис. 15](image/15.jpg){#fig:001 width=70%}

Просматриваю содержимое новой директории (рис. 15_1).

![рис. 15_1](image/15_1.jpg){#fig:001 width=70%}

Удаляю лишние файлы из директории work/study/2023-2024/Computer architecture/arch-pc/labs/lab04 (рис. 16).

![рис. 16](image/16.jpg){#fig:001 width=70%}

Совершаю commit директории (рис. 17).

![рис. 17](image/17.jpg){#fig:001 width=70%}

Загружаю файлы на Github (рис. 18).

![рис. 18](image/18.jpg){#fig:001 width=70%}



# Выводы

В результате выполнения работы получил практические навыки установки и использования ассемблера NASM в Linux Ubuntu для создания, трансляции, компоновки и запуска программ на низкоуровневом языке ассемблера.



# Список литературы

1. The NASM documentation. — 2021. — URL: https://www.nasm.us/docs.php.


::: {#refs}
:::
