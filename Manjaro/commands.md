# Установка пакетов
## Установка отдельных пакетов:
```console
$ pacman -S название_пакета1 название_пакета2 ... # установка одного пакета или списка пакетов
```

```console
$ pacman -U /путь_к_файлу/файл.tar.xz # установка пакета из файла
```
```console
$ pacman -U http://www.example.com/repo/example.pkg.tar.xz # или установка из сети
```
## Обновление
```console
$ pacman -Syu # установка пакета с обновлением системы
```

# Удаление пакетов
```console
$ pacman -R имя_пакета # удалить пакет
```
```console
$ pacman -Rs имя_пакета # удалить пакет с зависимостями (не используемыми другими пакетами)
```
```console
$ pacman -Rsc имя_пакета # удалить пакет с зависимыми и зависящами пакетами
```
```console
$ pacman -Rsn $(pacman -Qdtq) # удалить пакеты "сироты"
```

# Вызов help через терминал
```console
$ pacman -h # появится список флагов
```