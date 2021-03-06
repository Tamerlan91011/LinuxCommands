# Общие наиболее частые команды

## Только установил дистрибутив, или скачал пакет программ? Обновись!

```console
$ sudo apt update && sudo apt upgrade
```

**sudo** -  строка для активации режима "я тут главный и знаю, что делаю".

**apt** - пакетный менеджер для установки программ из открытых источников.

___

## "Кто я?"

Команда, помогающая узнать основные моменты про используемый дистрибутив:

```console
$ cat /etc/*release* # Сама команда
$ # Результат выполнения команды:
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=20.04
DISTRIB_CODENAME=focal
DISTRIB_DESCRIPTION="Ubuntu 20.04.4 LTS"
NAME="Ubuntu"
VERSION="20.04.4 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.4 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
```

___

## Команды навигации

### "Что тут лежит?"

Показать содержимое текущей директории:

```console
$ ls       # Для показа содержимого текущей дериктории
$ ls - l   # Для показа в виде таблицы со свойствами
$ ls - a   # Для показа скрытых папок
$ ls - al  # Для показа скрытых папок в виде таблицы
```

### "Где я?"

Показать адрес текующей директории:

```console
$ pwd
```

### "Как мне попасть туда?"

Переместиться в нужную директорию:

```console
$ cd folder_name    # Переместиться в директорию folder_name
$ cd ..             # Переместиться на уровень выше
```

___

## Команды взаимодействия с файлами

### "Как создать папку?"

```console
$ mkdir folder_name 
```

### "Как создать файл?"

```console
$ touch filename.txt # У файла обязателен формат
```

### "Как удалить папку, или файл?"

```console
$ rm filename       # Для удаления одного файла
$ rm -r foldername  # Для удаления папки с файлами внутри
```

### "Как двигать файлы, папки? А переименовать?"

```console
$ mv filename path/...     # Сначала выбираем файл, а потом указываем путь через пробел
$ mv filename new_filename  # Это переименовывание файла
```
___