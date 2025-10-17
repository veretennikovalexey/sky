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