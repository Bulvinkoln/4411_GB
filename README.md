# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## 1. Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у вас создаться репозиторий (появится скрытая папка .git)

## 2. Создание коммитов

Для добавления измений файл должен быть сохранен. Для добавления информации в коммит используется команда **git add**. Чтобы использовать команду **git add** напишите *git add <имя файла>*

### 3. Просмотр состояния репозитория
В состоянии репозитория отображаются все несохраненные изменения.
 Для того, чтобы посмотреть состояние репозитория используется команда **git status**. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### 4. Создание коммитов
Коммит это сохранение с комментарием о вносимых изменениях для удобного отслеживания проделанных изменения.
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду **git commit**. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Или воспользоваться командой *git commit -am "<cсообщение к коммиту>*. Так можно одноврменно добавить файл и сделать коммит.  Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## 5. Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда **git checkout**. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## 6. Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда **git log**. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## 7. Ветки в Git
Ветки в Git служат для работы над изменениями. Изменения могут вноситься как одним человеком, так и несколькими людьми, работающими над проектом.

### 8. Создание ветки

Для того, чтобы создать ветку, используется команда **git branch**. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## 9. Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## 10. Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## 11. Удаленный репозиторий
Удаленные репозитории используются различными участниками для работы над одним проектом. Также свои репозитории можно размещать на **git_hub.com** , если вы хотите продолжить на них работу с другого компьютера. Такой репозиторий также будет считаться удаленным.
## 12. Добавление удаленного репозитория.
Для того, чтобы добавить удалённый репозиторий и присвоить ему имя нужно выполнить команду *git remote add <имя репозитория> <адрес репозитория>*
Ссылку на адрес удаленного репозитория можно склонировать на сайте git_hub.com , нажав кнопку Code на выбранном репозитории.
## 13. Просмотр удаленных репозиториев
Для того, чтобы просмотреть список настроенных удалённых репозиториев, можно запустить команду **git remote**. Она выведет названия доступных удалённых репозиториев. 
## 14. Клонирование удаленного репозитория
Когда вы решаете поработать над уже существующим кодом, вы можете клонировать репозиторий с этим кодом. Для выполнения этой операции в Git предусмотрена команда **git clone**.
Для использования команды необходимо ввести *git clone <ссылка на удаленный репозиторий>*
## 15. Получение изменений из удаленного репозитория
Часто вместо этого хочется получать изменения и сразу обновлять рабочую копию так, чтобы она соответствовала удаленному репозиторию. И для этого в Git существует отдельная команда. Называется она **git pull**.
## 16. Отправка изменений в удаленный репозиторий
Для того , чтобы отправить изменения в удаленный репозиторий используется команда **git push**.
## 17. Работа с репозиторием на git_hub.com
Форк  – создает точную копия репозитория другого человека, но в вашем аккаунте. Форки нужны, чтобы вносить свои изменения в проект, к репозиторию которого у вас нет прямого доступа.

Пулл-реквест  – функция GitHub, позволяющая попросить владельца репозитория, от которого мы сделали форк, загрузить наши изменения обратно в свой репозиторий.
