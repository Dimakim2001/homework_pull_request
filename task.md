# Инструкция по работе с git репозиторием

## Для начала работы:
>git init

Если имя пользователя и почта еще не были заданы:

>git config -- global user.name

>git config --global user.email

## Работа с файлами:
Для того чтобы добавить файл, нужно:
1. git add file_name

добавляем файл с именем file_name для отслеживания

2. >git commit -m "some message"

* добавляем текущие изменения в репозиторий и подписываем их с помощью тега -m
* если добавить тег -а, то к комиту добавятся все измененные файлы , которые уже отслеживались

чтобы отслеживать состояние репозитория:
1. >git status
2. >git log
3. >git diff


## Работа с коммитами
Для того, чтобы перейти к определенному комиту можно использовать команду 
>git checkout code_comit
    code_comit - код комита к которому хотим перейти, его можно посмотреть в git log

Чтобы вернуться к самому последнему состоянию:
>git checkout master

![finish](finish.jpg)


## Ветки в git
Чтобы посмотреть все ветки:
> git branch

Для создания новой ветки с именем branch _name%
>git branch_name

Переместиться к ветке с именем branch_name%
>git checkout branch_name


## Слияние веток и решение конфликтов
Чтобы слить информацию из ветки branch_name в текущую:
>git merge branch_name


## Удаление веток
Для того, чтобы удалить ветку с именем branch_name:
>git branch -d branche_name

Удаление с игнорированием ошибок:
>git branch -D branch_name


## Справка

Чтобы вызвать справку по команде, допишите тег:
>--help

Примеры:
>git add --help

>git branch --help


## Удаленный репозиторий

Чтобы клонировать репозиторий:
>git clone

Чтобы отправить файл на удаленный репозиторий:
>git push

Чтобы скачать файл из удаленного репозитория:
>git pull


Чтобы авторизоваться:
> ssh-keygen -t rsa -b 4096 -c "dimakim2001@mail.ru"


