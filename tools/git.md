# Комманды для работы с git

## Начало работы с репозиторием

```console
$ git init # создать репозиторий в текущей папке

$ git init "repo_name" # создать новую папку с именем "repo_name" и создать в нем репозиторий

$ git init /path/to/repo/ # создать репозиторий в указанную директорию

$ git clone "/path/to/repo/" # скопировать локальный репозиторий в текущую директорию

$ git clone "https://repository_link" # скопировать удаленный репозиторий в текущую директорию
```

## Работа с ветками

```console
$ git branch #отображение существующих веток
$ git branch "branch_name" #создание новой ветки с именем "branch_name" (без кавычек)
$ git checkout "branch_name" # переключение на ветку с именем "branch_name"
```

## Удаление коммита (для GitHub)

```console
$ git reset --hard "commit-code"
$ git push --force
```

## Просмотр статистики репозитория
```console
$ git log # показывает историю коммитов текущей ветки 
$ git status # статус файлов в текущем репозитории
```