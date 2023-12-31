# Инструкция по работе с Git.

1. Создание репозитория:
```sh
git init
```
2. Отображение статуса текущего репозитория:
```sh
git status
```
3. Добавление файла к отслеживанию:
```sh
git add
```
пример: git add + имя файла

4. Выполнение фиксации файла в Git (коммит):
```sh
git commit -m "понятный осознанный комментарий, что было сделано"
```
5. Отображение истории зафиксированных коммитов (изменений):
```sh
git log
```
выводятся коммиты с индивидуальными номерами, авторами коммитов, электронной почтой авторов коммитов и датами коммитов

6. Отображение истории зафиксированных коммитов в укороченном виде (в одну строку):
```sh
git log --oneline
```
7. Перемещение по веткам сохраненных коммитов: данная команда предоставляет возможность переключаться на состояния, которые были зафиксированы ранее:
```sh
git checkout
```
* переключение по веткам с помощью идентификатора коммита, вместо звездочек необходимо ввести идентификатор коммита. Допускается вводить не весь идентификатор, а только первые семь символов.
```sh
git checkot *******
``` 
* команда, возвращающая на самое последнее состояние
```sh
git chechout master
```
8. Отображение различий между теми или иными коммитами:
```sh
git diff
```
* после команды git diff указываем ссылку на один коммит и через пробел ссылка на другой коммит, например git diff 15iu178 7s3hb45
9. Отображение всех веток:
```sh
git branch
```
10. Создание новой ветки:
```sh
git branch <имя_новой_ветки>
```
11. Визуальное отображение в консоли веток:
```sh
git log --oneline --graph
```
12. Слияние веток:
```sh
git merge
```
13. Удаление веток:
```sh
git branch -d <branch_name> 
```