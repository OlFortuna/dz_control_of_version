# Создали dz_control_of_version
# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создатся репозиторий (появится скрытая папка .git).
## Создание коммитов

### Git add
Для добавления измений в коммит(сохранение) используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*.
Для добавления всех существующих изменений: *git add .*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с репозиторием следующим образом: *git checkout <номер коммита>*. Или, например, можно перемещаться между ветками используя *git checkout <branch>*. 
Также с помощью команды *git checkout* можно создавать новые ветки:  *git checkout -b <branchname>*, или отменять изменения: *git checkout -- <file>*.

## Журнал изменений
Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием. Для просмотра изменений в сокращенном варианте: *git log --oneline*.
Для просмотра изменений веток в графическом прадставлении: *git log --graph*.
Для просмотра разницы между текущим файлом и закоммиченным файлом: *git diff*.

Этот текст введен через браузер

## Ветки в Git
Ветка в Git — это шкала последовательных коммитов, то есть ветка является местом повседневной работы разработчиков. Ветка может быть основной (main или master), то есть она будет отражает основной путь развития программы. Но также может быть неосновной. Такие ветки возникают, когда в основной ветке нужно решить какую-то проблему.

### Создание ветки
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*.
Для просмотра текущей ветки: *git branch*.

## Слияние веток
Для того чтобы добавить ветку в текущую ветку, используется команда *git merge <name branch>*.

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'".

