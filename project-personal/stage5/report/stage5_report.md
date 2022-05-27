---
## Front matter
title: "Отчёт по пятому этапу индивидуального проекта"
subtitle: "дисциплина: Операционные системы"
author: "Студент: Махорин Иван Сергеевич"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Добавить к сайту все остальные элементы.

# Задание

1. Сделать записи для персональных проектов.
2. Сделать пост по прошедшей неделе.
3. Добавить пост на тему: "Языки научного программирования".

# Выполнение индивидуального проекта

Чтобы сделать записи для персональных проектов мы должны проделать данный путь: "work", "blog", "content", "project", "example". Внутри каталога "example" мы открываем файл "index.md" (Рис. [-@fig:001]).

![Открытие нужного файла для редактирования](image/1.png){ #fig:001 width=100% }

Внутри файла меняем титульное название, а также ссылку на твитер меняем на GitHub. После чего добавляем этапы реализации нашего индивидуального проекта (Рис. [-@fig:002]).

![Редактирование файла проекта](image/2.png){ #fig:002 width=100% }

После этого проделаем путь для изменения презентации в проекте: "work", "blog", "content", "slides", "example". Внутри каталога "example" мы открываем файл "index.md" (Рис. [-@fig:003]).

![Открытие нужного файла для редактирования](image/3.png){ #fig:003 width=100% }

Внутри презентации добавляем тот же самый текст, который только что вносили в другой файл. А также добавляем ссылку на GitHub (Рис. [-@fig:004]).

![Редактирование файла презентации](image/4.png){ #fig:004 width=100% }

Теперь создадим каталоги для наших новых постов и назовём их: "Моя-4-неделя" и "Языки научного программирования". Чтобы создать эти каталоги нужно проделать следующий путь: "work", "blog", "content", "post" (Рис. [-@fig:005]).

![Создание каталогов для новых постов](image/5.png){ #fig:005 width=100% }

Добавим информацию для наших постов, которую мы написали заранее (Рис. [-@fig:006]).

![Добавление информации для поста "Языки научного программирования"](image/6.png){ #fig:006 width=100% }

Чтобы вся наша информация выгрузилась на сайт, откроем в каталоге "blog" терминал и запустим команду hugo (Рис. [-@fig:007]).

![Запуск команды hugo](image/7.png){ #fig:007 width=100% }

Как только команда hugo выполнилась перейдём первым этапом в подкаталог "public" и проделаем указанные на скриншоте действия (Рис. [-@fig:008]). Вторым этапом проделаем все те же самые действия, но уже в каталоге "blog" (Рис. [-@fig:009]).

![Выгрузка из подкаталога "public"](image/8.png){ #fig:008 width=100% }
	
![Выгрузка из каталога "blog"](image/9.png){ #fig:009 width=100% }

Последним шагом перейдём на наш сайт и посмотрим итог работы (Рис. [-@fig:010]), (Рис. [-@fig:011]) и (Рис. [-@fig:012]). 

![Новые посты](image/10.png){ #fig:010 width=100% }

![Записи для персональных проектов](image/11.png){ #fig:011 width=100% }

![Записи для персональных проектов](image/12.png){ #fig:012 width=100% }

# Выводы

В ходе выполнения пятого этапа индивидуального проекта мы научились добавлять к сайту все остальные элементы.
