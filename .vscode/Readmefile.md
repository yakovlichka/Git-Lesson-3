# ***Инструкция для работы с Git и удалёнными репозиториями***

# ***Что такое Git?***
# ***Git*** - ***это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.*** 

# ***Подготовка репозитория***
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## ***Создание коммитов***

### ***Git add***
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

## ***Просмотр состояния репозитория***

### ***Git status***
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

## ***Создание коммитов***

### ***Git commit***
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## ***Перемещение между сохранениями***

### ***Git checkout***
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## ***Журнал изменений***

### ***Git log***
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

# ***Ветки в Git***

## ***Создание ветки***

### ***Git branch***

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## ***Слияние веток***

### ***Git merge***
Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## ***Удаление веток***

### ***Git branch***

Для удаления ветки ввести команду "git branch -d 'name branch'"

# ***Работа с удаленными репозиториями***

## ***Добавление удаленных репозиториев***

### ***Git remote add***
Для того, чтобы добавить удалённый репозиторий и присвоить ему имя (shortname), просто выполните команду git remote add <shortname> <url>:

### ***Git pull***
Если ветка настроена на отслеживание удалённой ветки (см. следующий раздел и главу Ветвление в Git чтобы получить больше информации), то вы можете использовать команду git pull чтобы автоматически получить изменения из удалённой ветки и слить их со своей текущей. 

### ***Git push***
Когда вы хотите поделиться своими наработками, вам необходимо отправить их в удалённый репозиторий. Команда для этого действия простая: git push <remote-name> <branch-name>.

### ***Git remote show***
Если хотите получить побольше информации об одном из удалённых репозиториев, вы можете использовать команду git remote show <remote>. 