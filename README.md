# Домашнее задание к занятию " `Основы Git` " - `Сулименков Алексей`

---

## Задание 1. Знакомимся с GitLab и Bitbucket

### Добавление GitLab

<details> <summary>GitLab</summary>

```git
gitlab	git@gitlab.com:biparasite1/devops-netology.git (fetch)
gitlab	git@gitlab.com:biparasite1/devops-netology.git (push)
origin	https://github.com/biparasite/devops-netology.git (fetch)
origin	https://github.com/biparasite/devops-netology.git (push)
```

</details>

---

## Задание 2. Теги

Представьте ситуацию, когда в коде была обнаружена ошибка — надо вернуться на предыдущую версию кода, исправить её и выложить исправленный код в продакшн. Мы никуда не будем выкладывать код, но пометим некоторые коммиты тегами и создадим от них ветки.

1. Создайте легковестный тег v0.0 на HEAD-коммите и запуште его во все три добавленных на предыдущем этапе upstream.
2. Аналогично создайте аннотированный тег v0.1.
3. Перейдите на страницу просмотра тегов в GitHab (и в других репозиториях) и посмотрите, чем отличаются созданные теги.

### Ответ

1. [Github](https://github.com/biparasite/devops-netology/tags)
2. [Gitlab](https://gitlab.com/biparasite1/devops-netology/-/tags)

Аннотированный тег в gitlab отличается временем создания и равен дате коммита, в Github время добавления тега.

---

## Задание 3. Ветки

Давайте посмотрим, как будет выглядеть история коммитов при создании веток.

1. Переключитесь обратно на ветку main, которая должна быть связана с веткой main репозитория на github.
2. Посмотрите лог коммитов и найдите хеш коммита с названием Prepare to delete and move, который был создан в пределах предыдущего домашнего задания.
3. Выполните git checkout по хешу найденного коммита.
4. Создайте новую ветку fix, базируясь на этом коммите git switch -c fix.
5. Отправьте новую ветку в репозиторий на GitHub git push -u origin fix.
6. Посмотрите, как визуально выглядит ваша схема коммитов: https://github.com/YOUR_ACCOUNT/devops-netology/network.
7. Теперь измените содержание файла README.md, добавив новую строчку.
8. Отправьте изменения в репозиторий и посмотрите, как изменится схема на странице https://github.com/YOUR_ACCOUNT/devops-netology/network и как изменится вывод команды git log.

### Ответ

<details> <summary>git checkout </summary>

![git_checkout](https://github.com/biparasite/devops-netology/blob/main/git_checkout.png "git_checkout")

</details>

<details> <summary>git switch</summary>

![git_switch](https://github.com/biparasite/devops-netology/blob/main/git_switch.png "git_switch")

</details>

<details> <summary>git log</summary>

![git_log](https://github.com/biparasite/devops-netology/blob/main/git_log.png "git_log")

</details>

---

## Задание 4. Упрощаем себе жизнь

Попробуем поработь с Git при помощи визуального редактора.

В используемой IDE PyCharm откройте визуальный редактор работы с Git, находящийся в меню View -> Tool Windows -> Git.

Измените какой-нибудь файл, и он сразу появится на вкладке Local Changes, отсюда можно выполнить коммит, нажав на кнопку внизу этого диалога.

Попробуйте выполнить пару коммитов, используя IDE.

### Ответ

Использовал VSCODE

Два коммита

<details> <summary>git commit</summary>

![git commit](https://github.com/biparasite/devops-netology/blob/main/git_commit.png "git commit")

</details>
