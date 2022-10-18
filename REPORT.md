# Git-5-sem(lab-2)

## Задание 2

git checkout ci

git rebase -i HEAD~2

git checkout master

git cherry-pick ci

git branch -D ci

![Зад.2](https://github.com/poker303/Git-5-sem/blob/report/docs/task2.jpg)

## Задание 3

git reflog

git checkout aca3abb

git branch old-master

![Зад.3](https://github.com/poker303/Git-5-sem/blob/report/docs/task3.jpg)

## Задание 4

git blame prisma/seed.ts

![Зад.4](https://github.com/poker303/Git-5-sem/blob/report/docs/task4.jpg)

## Задание 5

npm install --save-dev jest

git checkout master

git bisect start

git bisect bad

git bisect good hash-code коммита, первого, чтобы интервалом поиска был весь репозиторий

npm run test

Eсли тест (`failed`), то пишем `git bisect bad`.

Eсли (`passed`), то `git bisect good`, а потом повторяем `npm run test`, пока не найдем первый bad commit.

![Зад.5](https://github.com/poker303/Git-5-sem/blob/report/docs/task5.jpg)

## Задание 6

git filter-branch --tree-filter "rm -f .env" -- --all

echo .env >> .gitignore

![Зад.6](https://github.com/poker303/Git-5-sem/blob/report/docs/task6.jpg)

## Задание 7

git checkout feature

git filter-branch --env-filter "GIT_AUTHOR_NAME='ФИО'; GIT_AUTHOR_EMAIL='ПОЧТА'; GIT_COMMITTER_NAME='ФИО'; GIT_COMMITTER_EMAIL='ПОЧТА'" HEAD~*количество_коммитов_до_разветвления_начала_разветвления*..HEAD

![Зад.7](https://github.com/poker303/Git-5-sem/blob/report/docs/task7.jpg)

## Задание 8

git checkout master

git config rerere.enabled true

git merge feature

Исправляем конфликты.

git add *file-name*

git commit --no-edit

git reset --hard HEAD~1

git merge feature

git add *file-name*

git commit --no-edit

![Зад.8](https://github.com/poker303/Git-5-sem/blob/report/docs/task8.jpg)

## Задание 9

git fsck

![Зад.9](https://github.com/poker303/Git-5-sem/blob/report/docs/task9.jpg)
