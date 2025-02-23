# Инструкция по работе с git
![Официальный логотип git](logo.png)

## Lesson 1

## Что такое git и контроль версий
**Системы контроль версий** - это системы, которые: 
1. обеспечивают сохранение содержимого файлов и папок(их *версий*)
2. Обеспечивают передвижение по *версиям* этих файлов и папок

**git** - это самая известная и используемая на данный момент реализация контроля версий с командным интерфейсом

**Локальный репозиторий** - это хранилище *изменений* Git в виде папки.

## Инициализация локального репозитория

Для того чтобы сказать git, что данная папка является локальным репозиторием нужно зайти в папку и ввести в ней команду

*git init*

Также, если этого раньше не делалось, то нужно определить ваше имя пользователя и email командами:
. git config --global user.name "your name"
. git config --global user.email your email 

## Добавление файлов под контроль версий

Для этого нужно ввести команду:
*git add имена файлов*
Теперь имена и содержимое этих файлов можно сохронять

## Делаем коммит

Для того, чтобы изменения представляли собой отдельную версию, к которой можно возвращаться и манипулировать после добавления под **контроль версий**, нужно ввести команду:

*git commit -m "Название версии"*

Можно также добавить под контроль версий и сформировать коммит для всех  файлов и папок одной командой:
*git commit -am "Название версии"

## Просмотр текущего состояния репозитория
Для вывода текущего состояния локального репозитория используются команды:

>git status - просмотр состояния файлов и папок в репозитории

> git diff - просмотр самих изменений файлов и папок

## Просмотр всех изменений репозитория

Для просмотра истории изменений от начала и последнего коммита нужно ввести:

*git log*

git status - команда, вывод состояния репозитория
git init - иницыализация git
## Lesson 2
git branch - выводит ветки
branch
git branch name - создание ветки
Github

## Работа с удаленным репозиторием
Для работы с удаленным репозиторием необходимо зарегистрироваться на сайте github.com.
Затем создать там новый репозиторий или клонировать существующий.

Для создания нового удаленного репозитория и загрузки актуальных версии файлов из локального репозитория в удаленный надо воспользоваться следующими командами 
* git remote add origin https://https://github.com/lyapdy/Test-Git.git
* git branch -M master 
* git puch -u origin master


Для работы в локальном репозитории необходимо воспользоваться командой git pull, чтобы загрузить актуальные файлы в локальный репозиторий. Предварительно нужно создать папку, в которой эти файлы будут находиться в локальном репозитории. Затем нажать кнопку "Клонирование репозитория github" и указать созданную папку.