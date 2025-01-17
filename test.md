 # Инструкция по работе с Git-ом 

## Инициализация репозитория

> **git init** - создание пустого репозитория в выбранной папке.

## Работа с репозиторием

> **git add .** - сохранить все файлы, которые были добавлены в репозиторий. Добавили **30** картинок - "git add ." сохранит все 30 файлов сразу

> **git add** - сохранить один файл, записанный в репозиторий

> **git commit -m "message"** - создание коммита, где **-m** - сокращение от **"message"** и **"message"** является комментарием к файлу

## Работа с коммитами

> **git log** - вывод на экран списка всех коммитов с хеш-кодами (уникальный номер, по которому можно отследить коммит)

> **git checkout** - переход между коммитами

> **git checkout master** - вернуться к актуальному состоянию и продолжить работу

> **git diff** - вывод разницы между текущим файлом и последним коммитом

## Синтаксис языка Markdown

### Заголовки

> Знаком ( # ) в начале строки можно выделить заголовок (поддерживается до 6 уровней). Например:

> # Заголовок первого уровня
> ## Заголовок второго уровня
> ### Заголовок третьего уровня
> #### Заголовок четвертого уровня

> И так далее. Также можно использовать знаки ( = ) или ( - ) ( не менее 3 подряд ) для выделения заголовков первого ("=") и второго ("-") уровней.

> вот так
> ===

> и так
> ---

### Выделение текста

> Чтобы выделить текст курсивом необходимо обрамить его звездочками ( * ) или знаком нижнего подчеркивания ( _ ). Например, *вот* или _вот так_.

> Чтобы выделить текст полужирным необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания(__). Например, **вот** или __вот так__.

> Альтернативные способы выделения текста курсивом или жирным нужны для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен **курсивом и при этом быть полужирным**_.

> Для написания "зачеркнутого текста" можно использовать двойной символ (**~**). Например, ~~вот так~~

### Списки

> Чтобы добавить ненумерованные списки необходимо пункты выделить звездочкой (*) или знаком +. Например:
> * Элемент 1
> * Элемент 2
> * Элемент 3
> + Элемент 4

> Чтобы добавить нумерованные списку, необходимо пункты пронумеровать. Например:
> 1. Первый пункт
> 2. Второй пункт

## Работа с изображениями

> Чтобы вставить изображение в текст, достаточно написать следующее:
![Это Кисик!](Kisik.jpg)

## Продолжение работы с коммитами

> **git log --graph** – журнал коммитов с визуализацией веток в которых был конфликт

> **git commit -am “текст_коммита”** - добавление изменения файла и его коммит одной командой

## Работа с слиянием веток

> **git merge <Название ветки>** - заносит информация из названной ветки в используемую на данный момент

## Работа с ветками

> **git branch** – посмотреть список веток в репозитории

> **git branch <название ветки>** – проверка существования ветки с таким именем и если такой ветки несуществует, происходит ее создание.

> **git checkout <название ветки>** – переход к ветке с указанным названием

> **git branch -d <название ветки>** - проверка существования ветки с таким именем и если такая ветка существует, происходит ее удаление

> **git checkout -b branch_name** - создание ветки и переход  в нее одной командой

## Инструкция по связке GIT - GITHUB

Чтобы склонировать репозиторий к себе на ПК, используется команда:
> **git clone URL** https://github.com/Krekeloid/A.S__BRAVE5173.git - клонируется репозиторий по адресу **URL**

> **git pull** – получение изменений с GITHUB и слияние с файлом, который находится на ПК

> **git push** - отправляет репозиторий с ПК на GITHUB 