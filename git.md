# Основы Git

## 1.4 Первый репозиторий 

git init создаёт локальный репозиторий в текущей папке

Появляется новая подпапка .git которая хранит информацию о коммитах

mkdir first_project

ls

cd first_project

pwd

ls -la

git init

cd .git

cat config

git config user.name veretennikovalexey

git config --global user.name

git config user.name

git config --list

git config list --global

git config list --local

cd -

cd c:/Users/Pragmatic_Programmer

cat .gitconfig

## 1.5 Первый коммит

git status

git log

cat page1.html

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <h1>My first Heading</h1>
        <p>My first paragraph.</p>
        <p>My second paragraph.</p>
    </body>
</html>
```

git add page1.html

git commit

## 1.6 Индекс

Индекс или stage это шлюз между космосом и космическим кораблём

Один и тот же файл может быть модифицирован 2 раза, а в индекс может попасть только первое изменение

git reset --hard

## 1.7 Подробнее о коммитах

git commit -a

git commit --amend

git show

git show <commit_id>

git show --name-only <commit_id>

git reset HEAD~1

git commit -m "add some new features"

git commit -am "add some new features"

## 1.8 Откат изменений

git reset

git reset <file_name>

git reset --hard

git reset HEAD~1
git reset HEAD^

git reset HEAD~2
git reset HEAD^^

git reset HEAD~3
git reset HEAD^^^

git reset HEAD~2 --hard

cat .git/ORIG_HEAD

git reset ORIG_HEAD --hard

git reset --hard <commit_id>

git log --oneline

git revert

git revert --help

git show

git revert HEAD

cat styles.css

git revert HEAD --no-edit

git revert 8ab14c

git revert HEAD~3

git revert --abort

git revert 9e59768..4b2413e

git revert 9e59768 --no-commit

## 1.9 Удаление файлов

git rm --help

rm page2.html

git rm page2.html

git rm page2.html -f
git rm page2.html --force

git rm my_folder -r
git rm my_folder --recursive

git clean --help

touch some_binary_file{1..9}.bin
ls

git status

git clean -f
ls
git status

mkdir bin
mkdir tmp
ls

git status

git clean -d -f
ls
git status

git clean -f -n
git clean -f -d -n

git clean -f -d -q

## 1.10 Переименование/перемещение файлов

mv page1.html index.html

mv page1.html index.html
git add index.html
git rm page1.html

git mv page1.html index.html

git mv --help

mkdir styles

git mv styles.css styles

git commit -m "create folder for css styles"

git mv styles css

mkdir web_pages

git mv *.html web_pages

## 1.11 Просмотр изменений

