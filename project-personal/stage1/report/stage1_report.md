---
## Front matter
title: "Отчёт по первому этапу индивидуального проекта"
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

Разместить на Github pages заготовки для персонального сайта.

# Задание

1. Установить необходимое программное обеспечение.
2. Скачать шаблон темы сайта.
3. Разместить его на хостинге git.
4. Установить параметр для URLs сайта.
5. Разместить заготовку сайта на Github pages.

# Выполнение лабораторной работы

Скачаем исполняемый файл hugo на сайте https://github.com/gohugoio/hugo/releases. Нам нужен архив hugo_extended_0.98.0_Linux-64bit.tar.gz (рис. [-@fig:001]).

![Скачивание исполняемого файла](image/1.png){ #fig:001 width=70% }

В разделе "Загрузки" извлекаем файлы из архива в текущую папку (рис. [-@fig:002]).

![Разархивация](image/2.png){ #fig:002 width=70% }

В домашнем каталоге создаём каталог "bin", после чего переходим в него и вставляем "hugo" (hugo мы скопировали из разархивированной папки) (рис. [-@fig:003]).

![Создание каталога "bin" и перенос в него "hugo"](image/3.png){ #fig:003 width=70% }

Создаём новый репозиторий "blog" при помощью шаблона (рис. [-@fig:004]).

![Новый репозиторий](image/4.png){ #fig:004 width=70% }

Далее возвращаемся в терминал и переходим в каталог "work", в который клонируем наш новый репозиторий. После чего переходим в наш новый каталог "blog" (рис. [-@fig:005]).

![Клонирование репозитория](image/5.png){ #fig:005 width=100% }

В каталоге "blog" производим установку "go" (рис. [-@fig:006]).

![Установка "go"](image/6.png){ #fig:006 width=70% }

Выполняем команду "~/bin/hugo" (рис. [-@fig:007]).

![~/bin/hugo](image/7.png){ #fig:007 width=100% }

Вводим команду "mc" и выполняем удаление каталога "public" (рис. [-@fig:008]).
	
![Удаление каталога "public"](image/8.png){ #fig:008 width=70% }

После успешного удаления и возвращения в терминал, вводим команду "~/bin/hugo server" и получаем ссылку на наш локальный сайт (рис. [-@fig:009]).

![Получение ссылки на локальный сайт](image/9.png){ #fig:009 width=100% }

Переходим на этот сайт через браузер (рис. [-@fig:010]). 

![Просмотр локального сайта](image/10.png){ #fig:010 width=100% }

На сайте мы видим предупреждение, которое требуется убрать. Для этого мы переходим в файлы домашнего каталога и выполняем следующий путь: "work", "blog", "content", "home". После чего удаляем файл "demo.md" (рис. [-@fig:011]).

![Удаление файла "demo.md"](image/11.png){ #fig:011 width=70% }

Снова переходим на github и создаём еще один репозиторий, но уже со специальным названием (Ivan-Mahorin.github.io) (рис. [-@fig:012]). 
    	
![Создания репозитория со специальным названием](image/12.png){ #fig:012 width=100% }

Возвращаемся в терминал и переходим в каталог "work". В него мы клонируем наш репозиторий. Выполняем проверку с помощью команды "ls -l" (рис. [-@fig:013]). 

![Клонирование репозитория и выполнение проверки](image/13.png){ #fig:013 width=70% }

Переходим в наш новый каталог и переключаемся на ветку "main". Создаём пустой файл и отправляем его на github для активации нашего репозитория (рис. [-@fig:014]).

![Создание пустого файла и добавлени его на github](image/14.png){ #fig:014 width=100% }

Снова возвращаемся в терминал и переходим в каталог "blog". Выполняем команду для подключения нашего каталога "public" к новому репозиторию (рис. [-@fig:015]).

![Попытка подключения](image/15.png){ #fig:015 width=100% }

Запускаем команду "mc", далее находим ".gitignore" и переходим в него. Комментируем "public" (рис. [-@fig:016]).

![Комментирование "public"](image/16.png){ #fig:016 width=100% }

С помощью команды "cat .gitignore" выполняем проверку, после чего повторяем действия с подключением каталога (рис. [-@fig:017]).

![Подключение каталога к новому репозиторию](image/17.png){ #fig:017 width=100% }

С помощью команды "~/bin/hugo" генирируем автоматически файлы в папку "public"  (рис. [-@fig:018]).

![Автоматическая генирация файлов](image/18.png){ #fig:018 width=100% }

Синхронизируем файлы из каталога "public" с репозиторием. Для этого переходим в каталог "public" и проверяем подключение этого каталога к репозиторию. После этого проделываем стандартные действия с выгрузкой файлов в наш репозиторий (рис. [-@fig:019]).

![Проверка подключения каталога и выгрузка файлов в репозиторий](image/19.png){ #fig:019 width=100% }

Переходим на github и обновляем страницу репозитория (рис. [-@fig:020]).

![Обновление репозитория](image/20.png){ #fig:020 width=100% }

Копируем ссылку на наш новый сайт и переходим на него (рис. [-@fig:021]).

![Переход на сайт](image/21.png){ #fig:021 width=100% }

# Выводы

В ходе выполнения первого этапа индивидуального проекта мы научились размещать на Github pages заготовки для персонального сайта.

