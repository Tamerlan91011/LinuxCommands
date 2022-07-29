# Команды для работы с Python в среде Linux

## Виртуальное окружения проекта Python

Для создания виртуального окружения проекта на Python в ОС Linux необходимо прописать следующую команду:

```console
$ python3 -m venv env_name 
```

Для активации виртуального окружения:

```console
$ source env_name/bin/activate
```

Для деактивации:

```console
$ deactivate
```

Для сохранения модулей виртуального окружения НЕ нужно сохранять весь пакет `venv`.

Для этого достаточно сохранить список необходимых зависимостей в текстовый документ, который и будет сохранет в Git:

```console
$ pip freeze > requirements.txt
```

А чтобы потом установить эти зависимости, нужно прописать следующую команду:

```console
$ pip install -r requirements.txt
```

---

## Команды пакетного менeджера pip

Посмотреть список установленных пакетов в текущем виртуальном окружении (либо в текущем интерпретаторе ОС):

Обновление пакетного менеджера:

```console
$ pip install --upgrade pip
```

Отобразить список установленных в виуртальном окружении пакетов:

```console
$ pip list 
```

Установить пакет:

```console
$ pip install package-name
```

Удалить пакет:

```console
$ pip uninstall package-name
```