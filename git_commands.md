# Основные команды git

## Работа с конфигурацией
Типы настроек (property_type):
- Системная (`--system`)
- Пользовательская (`--global`)
- Для репозитория (`--local`)
#### Установить имя
```sh
$ git config --global user.name [name]
```
#### Установить почту
```sh
$ git config --global user.email [email]
```
#### Получить все настройки
```sh
$ git config --list
```
Настройки снизу переопределяют те, что вверху
#### Откуда именно взяли настройку
```sh
$ git config --show-origin [property_name]
```
#### Удалить настройку
```sh
$ git config [property_type] --unset [property_name]
```

## Работа с репозиторием

#### Создать локальный репозиторий

```sh
$ git init
```

#### Клонировать удаленный репозиторий

```sh
$ git clone [url]
```


Чтобы клонировать в папку с произвольным именем:

```sh
$ git clone [url] [folder_name]
```
#### Добавить удаленный репозиторий
```sh
$ git remote add [repository_name] [url]
```
#### Удалить удаленнный репозиторий
```sh
$ git remote remove [repository_name]
```
#### Просмотреть список удаленных репозиториев
```sh
$ git remote -v
```

## Состояние репозитория
#### Просмотреть статус файлов в репозитории
```sh
$ git status
```

## Работа с файлами в репозитории
#### Подготовить файлы к коммиту
```sh
$ git add [file or folder]
```
#### Удалить файл из репозитория
```sh
$ git rm [file or folder]
```
#### Переименовать (переместить) файл в репозитории
```sh
$ git mv [from] [to]
```

## Работа с ветками
#### Создать новую ветку от текущей ветки
```sh
$ git branch [new branch name]
```
#### Создать новую ветку от текущей ветки и сразу перейти на неё
```sh
$ git checkout -b [new branch name]
```

## Полезные ресурсы
* [https://git-scm.com](https://git-scm.com) - основная страница git
* [Learn Enough Git to Be Dangerous](https://www.learnenough.com/git-tutorial) - Книга Майкла Хартла, посвященная Git с самых основ
* [Pro Git](https://git-scm.com/book/ru/v2) - великолепная книга Скотта Чакона и Бена Страуба про Git
* [Git Internals](https://github.com/pluralsight/git-internals-pdf) - еще одна великолепная книга Скотта Чакона, посвященная Git