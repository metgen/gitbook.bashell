---
description: cp (copy)
---

# Команда cp в Linux

Команда сp используется для копирования файлов и папок из одного каталога в другой.

### Синтаксис и опции cp в Linux

Утилита cp имеет два следующих синтаксиса:

> Копирование файла в папку назначения с задание имение копируемого файла

```bash
cp опции /путь/к/файлу/источника /путь/к/файлу/назначения
```

> Копирование файла сохранение его имени в указанную папку

```bash
cp опции /путь/к/файлу/источника /путь/к/директории/назначения
```

Опции для команды cp:

* **--attributes-only** - не копировать содержимое файла, а только флаги доступа и владельца;
* **-b, --backup** - создать резервную копию файла назначения если он существует;
* **--copy-contents** - копировать содержимое для специальных файлов (сокеты, файлы устройств);
* **-f, --force** - удалить файл назначения перед попыткой записи в него если он существует;
* **-i, --interactive** - спрашивать, нужно ли перезаписывать существующие файлы;
* **-n, --no-clobber** - не перезаписывать существующие файлы;
* **-P**, **--no-dereference** - копировать сами символические ссылки, а не то на что они указывают;
* **-L**, **--dereference** - копировать не символические ссылки, а то, на что они указывают;
* **-l, --link** - создавать жесткие ссылки вместо копирования;
* **--preserve** - переносить указанные атрибуты с файла источника в файл назначения, возможные значения: **mode, ownership, time‐stamps, context, links, xattr, all**;
* **--no-preserve** - не переносить указанные атрибуты;
* **--parents** - сохранять путь, указанный в файле источнике, в папке назначения;
* **-r**, **--recursive** - копировать папку Linux рекурсивно;
* **--reflink** - использовать Copy on Write если это поддерживается файловой системой;
* **-s**, **--symbolic-link** - не выполнять копирование файлов в Linux, а создавать символические ссылки;
* **-S**, **--suffix** - указать суффикс для резервных копий файлов;
* **--sparse** - настройка работы с разреженными файлами;
* **-t**, **--target-directory** - считать файл-назначения директорией и копировать файл-источник или директорию-источник в эту директорию с оригинальным именем;
* **-T, --no-target-directory** - считать директорию назначения файлом или директорией для записи данных. Если в качестве источника выбран файл, то он будет скопирован с новым именем. Если директория, то её содержимое будет скопировано в директорию назначения;
* **-u**, **--upgrade** - скопировать файл, только если он был изменён;
* **-x**, **--one-file-system** - рекурсивное копирование не должно выходить за пределы этой файловой системы;
* **-v**, **--verbose** - максимально подробный вывод.

Также существуют опции, которые объединяют в себе несколько других с определёнными значениями. Во основные из них:

* **-p** — сохранять владельца, временные метки и флаги доступа при копировании, аналогично —**preserve=mode,ownership,timestamps**;
* **-d** — копировать символические и жесткие ссылки именно как ссылки, аналогично **—no-dereference —preserve=links**;
* **-a** — режим резервного копирования, при котором сохраняются все атрибуты, ссылки, а также выполняется резервное копирование папок, аналогично **—recursive —preserve=all, —no-dereference**;

### Практика
