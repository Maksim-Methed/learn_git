# git-config
## Действия после установки git

git config --list # посмотреть настройки

git config --global user.name “имя”
git config --global user.email “почта”


git config --global core.safecrlf warn
git config --global core.quotepath off
git config --global init.defaultBranch main # Ветка по умолчанию

### windows
git config --global core.autocrlf true


### MAC & UNIX
git config --global core.autocrlf input





## Действия при инициализации нового репозитория и при работе с ним

git init  инициализация git репозитория

git status  текущее состоянеие репозитория

git add index.html  добавить в трек (отслеживаемые) файл или папку

git add .  добавить все файлы из корня в трек

git commit -m "сообщение"  выполнить коммит (сделать слепок) текущего состояния проекта

git log --oneline  посмотреть историю коммитов

git diff # показывает изменения
git diff --color-words # показывает по строкам изменения

## отменить коммит "ПЕРЕПИСЫВАЕТ ИСТОРИЮ"
git reset 'HASH commit' - вернуться к коммиту старому но оставить текущие изменения
git reset --hard 'HASH commit' - вернуться к коммиту и удалить все изменения

git checkout .  откатить изменения у всех файлов трека
git checkout name.file # откатить изменения в одном файле или каталоге

### отправить изменения в удаленный репозиторий
```Shell Session
git push 
```

### клонирование репозитория
```Makefile
git clone https://github.com/Quper87/git-lesson.git
```

### сохраняет изменения отслеживаемых файлов и выполняет коммит
```shell
git commit -a -m 'сохраняет изменения отслеживаемых файлов и выполняет коммит'
```
