# git-config

git config --global user.name “Максим Лескин”
git config --global user.email “Quper87@gmail.com”

git config --list # посмотреть настройки

git config --global core.autocrlf true
git config --global core.quotepath off
git config --global core.safecrlf warn
git config --global init.defaultBranch main

git init # инициализация репозитория
git add . # добавить все файлы в track
git commit -m "описание" # сделать коммит