## Домашнее задание к занятию «Инструменты Git»

## Шкутов Иван Владимирович

### Задание

В клонированном репозитории:

1. Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.

2. Ответьте на вопросы.
   
- Какому тегу соответствует коммит 85024d3?
 
- Сколько родителей у коммита b8d720? Напишите их хеши.

- Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.

- Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...) (вместо троеточия перечислены аргументы).

- Найдите все коммиты, в которых была изменена функция globalPluginDirs.

- Кто автор функции synchronizedWriters?

В качестве решения ответьте на вопросы и опишите, как были получены эти ответы.



1. Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.

git show aefea 

git log aefea

![1](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/1.png)

![2](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/2.png)

Полный хеш коммита: aefead2207ef7e2aa5dc81a34aedf0cad4c32545

Комментарий к коммиту: Update CHANGELOG.md

2. Ответы:

- Какому тегу соответствует коммит 85024d3?

git log 85024d3 --oneline

коммиту 85024d3 соответствует tag v0.12.23  

![3](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/3.png)


- Сколько родителей у коммита b8d720? Напишите их хеши.

git log b8d720 --pretty=format:'%h %s' --graph

![6](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/6.png)

Проверка наличия первого родителя: git show b8d720^1

![7](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/7.png)

Проверка наличия второго родителя: git show b8d720^2

![8](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/8.png)

Проверка наличия третьего родителя: git show b8d720^3. Третьего родителя нет.

![9](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/9.png)

Хеши родителей коммита b8d720: 1 - 56cd7859e05c36c06b56d013b55a252d0bb7e158, 2 - 9ea88f22fc6269854151c571162c5bcf958bee2b.


- Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.

git log v0.12.23..v0.12.24 --oneline

![10](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/10.png)

![11](https://github.com/Ivan-Shkutov/git-homeworks-04/blob/main/11.png)


- Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...) (вместо троеточия перечислены аргументы).




- Найдите все коммиты, в которых была изменена функция globalPluginDirs.






- Кто автор функции synchronizedWriters?





