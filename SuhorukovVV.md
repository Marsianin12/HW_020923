# Краткое руководство по Git
## Основные команды
* git init - создаёт репозиторий
* git add - добавить файл
* git commit - фиксация изменений
* git diff - показать изменения
* git log - показать список "фиксаций"
## Работа с ветками
* git branch - выводит список веток
* git branch branch_name - создание ветки с именем branch_name
* git checkout branch_name - переход на ветку с именем branch_name
* git checkout -b branch_name - переход на созданную ветку branch_name
* git merge branch_name - добавляет ветку branch_name к той, на которой мы находимся
* git baranch -d branch_name - удаляет ветку с именем branch_name
* git log --graph - показывает ветвления с коммитами
* git reset HEAD~ - удаляет коммит
* git reset --hard HEAD~ - удаляет коммит и изменения
## Работа с удалёнными репозиториями