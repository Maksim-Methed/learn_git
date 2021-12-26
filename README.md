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

### текущее состояние репозитория
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

# GIT LVL 2

### Получение изменений с Github
```shell
git pull --rebase
```

### Восстановление файла
```shell
git restore index.js
```

### Восстановление файла
```shell
git log # логи
git log -p # логи с diff
```

### Посмотреть коммиты файла
```shell
git blame README.md
```

### Поиск подстроки в файлах
```shell
git grep строка
```


### Откатить изменения до коммита
```shell
git reset
git reset --hard HEAD~
```

### Дописать последний коммит
```shell
git commit --amend
```


### путешествие по коммитам
```shell
git checkout <хеш коммита>
git checkout main # вернуться
```

### путешествие по коммитам
```shell
git stash # убрать в stash
git stash pop # достать из stash
```

git log --graph # просмотр в виде графика
git log --graph --oneline # просмотр в виде удобного графика

### работа с ветками
```shell
git checkout -b {имя ветки} # создать новую ветку
git checkout main # перейти в ветку
git merge {имя ветки} # слить ветку
```
