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
