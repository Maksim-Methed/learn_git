# git-config
## Действия после установки git

### посмотреть настройки
```shell
git config --list
```

```shell
git config --global user.name “имя”
git config --global user.email “почта”


git config --global core.safecrlf warn
git config --global core.quotepath off
git config --global init.defaultBranch main # Ветка по умолчанию
```

### windows
```shell
git config --global core.autocrlf true
```


### MAC & UNIX
```shell
git config --global core.autocrlf input
```


## Действия при инициализации нового репозитория и при работе с ним


### инициализация git репозитория
```shell
git init
```

### текущее состоянеие репозитория
```shell
git status
```

### добавить в трек (отслеживаемые) файл или папку
```shell
git add index.html
```

### добавить все файлы из корня в трек
```shell
git add .
```

### выполнить коммит (сделать слепок) текущего состояния проекта
```shell
git commit -m "сообщение"
```

```shell
git log --oneline  посмотреть историю коммитов

### показывает изменения
```shell
git diff
git diff --color-words // показывает по строкам изменения
```

## отменить коммит "ПЕРЕПИСЫВАЕТ ИСТОРИЮ"

### вернуться к коммиту старому но оставить текущие изменения
```shell
git reset 'HASH commit'
```

### вернуться к коммиту и удалить все изменения
```shell
git reset --hard 'HASH commit'
```
### откатить изменения у всех файлов трека
```shell
git checkout .  
git checkout name.file  // откатить изменения в одном файле или каталоге
```

### откатить изменения в одном файле или каталоге
```shell
git checkout name.file
```

### отправить изменения в удаленный репозиторий
```shell
git push 
```

### клонирование репозитория
```shell
git clone https://github.com/Quper87/git-lesson.git
```

### сохраняет изменения отслеживаемых файлов и выполняет коммит
```shell
git commit -a -m 'сохраняет изменения отслеживаемых файлов и выполняет коммит'
```
