# Краткое руководсво по GIT
## 1. Основные комманды
* clear - очистить окно консоли
* git init - создает репозиторий
* git status - отображение статуса ветки
* git add - добавить файл для отслеживания
* git commit - сохранить текущее состояние
    * -a - сохранить все изменения
    * -m - комментарий
    ```powershell
    git commit -a -m "Your message"
    ```
* git diff - различе между версиями
* git log - лог изменений
    * q - выйти из отображения журнала
    ```powershell
    git log
    Author: Илья Смаль <johngoblikon328@gmail.com>
    Date:   Sat Sep 2 18:29:45 2023 +1000

        Added git init descr

    commit 185c1960c0fdb07063679f46adc4046ab6cdcd2a
    Author: Илья Смаль <johngoblikon328@gmail.com>
    Date:   Sat Sep 2 18:21:27 2023 +1000

        Added SubHeader

    commit d991bd919361629b0c9bebd4afbb1f74ad205e9e
    Author: Илья Смаль <johngoblikon328@gmail.com>
    Date:   Sat Sep 2 18:18:35 2023 +1000
    ```
* git checkout - переход между версиями

## 2. Работа с ветками

* git branch - вывести список веток ( * отмечена текущая ветка)
    ```powershell
    $ git branch 
    * branches
    headers
    master
    ```
* git branch branch_name - создать ветку с именем branch_name
* git checkout branch_name - переключиться на ветку branch_name
* git merge branch_name - перенести изменения из ветки branch_name в текущую ветку

## 3. Команды для упрощенной работы

* git checkout -b branch_name - создать ветку с именем branch_name и переключиться на неё
* git commit -a -m "Your message" - добавление измененных файлов для отслеживания, коммит и комментарий к коммиту
    * -a - сохранить все изменения
    * -m - комментарий
* git commit -am "Your message"
* git log --graoh - лог изменений с визуальным отображением коммитов и веток
$ git log --graph
    ```powershell
    *   commit 4c802254a460183a7f3f62388b5d16051346a51a (HEAD -> master)
    |\  Merge: b1ee6c1 dcf2499
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:31:56 2023 +1000
    | |
    | |     Merge branch 'extended_commands'
    | |
    | * commit dcf2499e7e3d21e0daf307fac00a2d2cf0fd0ccd (extended_commands)
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:26:01 2023 +1000
    | |
    | |     git commit another example added
    | |
    | * commit 813f24189c2b9b1b41367cbe91c5829b332639f4
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:25:10 2023 +1000
    | |
    | |     Commands added
    | |
    | * commit 309d9f80224bd62806a639e183e4e36267984cff
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:24:39 2023 +1000
    | |
    | |     Added header
    | |
    * | commit b1ee6c1943f89945ea2000adbdc9bf298224d334 (branches)
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:22:29 2023 +1000
    | |
    | |     git branch description modified
    | |
    * | commit 9cbd001aabe9f3f05c2181a5e1f221cc591d79ae
    | | Author: Илья Смаль <johngoblikon328@gmail.com>
    | | Date:   Sun Sep 10 16:21:23 2023 +1000
    | |
    | |     Commands added
    | |
    * | commit 8f76a7e0460641a2198dfd313b4761f0e2be9ffe
    |/  Author: Илья Смаль <johngoblikon328@gmail.com>
    |   Date:   Sun Sep 10 16:19:44 2023 +1000
    |
    |       Added header
    |
    * commit ddcb2203036b9045c1805345d08b51f4d44868e1
    | Author: Илья Смаль <johngoblikon328@gmail.com>
    | Date:   Sun Sep 3 15:31:45 2023 +1000
    |
    |     Added git-status, links, examples
    |
    * commit a0d025000c0183cbfd0696437454d4d39c7a2161
    | Author: Илья Смаль <johngoblikon328@gmail.com>
    | Date:   Sun Sep 3 15:11:31 2023 +1000
    |
    |     Added git commands
    |
    * commit c44342da63df5272805acde43538f28f0e297794
    | Author: Илья Смаль <johngoblikon328@gmail.com>
    | Date:   Sat Sep 2 18:29:45 2023 +1000
    |
    |     Added git init descr
    |
    * commit 185c1960c0fdb07063679f46adc4046ab6cdcd2a
    | Author: Илья Смаль <johngoblikon328@gmail.com>
    | Date:   Sat Sep 2 18:21:27 2023 +1000
    |
    |     Added SubHeader
    |
    * commit d991bd919361629b0c9bebd4afbb1f74ad205e9e
    | Author: Илья Смаль <johngoblikon328@gmail.com>
    | Date:   Sat Sep 2 18:18:35 2023 +1000
    |
    |     Added head
    |
    * commit 80b11556a82f7fed68f809930401e0f0b04a79cb
    Author: Илья Смаль <johngoblikon328@gmail.com>
    Date:   Sat Sep 2 18:06:45 2023 +1000

        Initial commit
    ```

## 4. Работа с удалённымии репозиториями

* git clone <https://linkexample.com/test.git> - клонировние внешнего репозитория на ПК
* git pull - скачивание изменений из текущего репозитория и автоматичское слияние
* git push - отправка версии на внешний репозиторий


## 5. Документация по GIT
<https://git-scm.com/docs>

## 6. Дистрибутивы GIT
<https://git-scm.com/downloads>