# Инструкция по работе с Git и GitHub


## Что такое система контроля версий?

## что такое git?
Git - это одна из реализаций распределённых систем контроля версий. Git Позволяет управлять нашими изменениями, создавать фиксации, ветки, а так же сливать их.

## Подготовка репозитория
Репозиторий - это хранилище файлов, поддерживающее версионность. Создать репозиторий можно с помощью применения в папке команды *git init*

## Создание сохранений

Мы можем создавать "сохранения" наших версий файлов. Такие "сохранения" называются фиксациями или коммитами. Сделать коммит можно с помощью команды *git commit* и **ОБЯЗАТЕЛЬНО** использовать флаг *-m* после чего в кавычках написать сообщение

## Журнал изменений

## Перемещение между сохранениями
Перемещаться между нашими "сохраниями" можно с помощью команды *git checkout*. Для этого достаточно применить команду *git checkout <номер коммита>*. 
Можно отменить изменения с помощью с помощью команд *git revert* и *git reset*
*git revert <номер коммита>* отменет изменения до указанной версии и создаст новый коммит.
*git reset --hard <номер коммита>* отменит изменения до указанного коммита и затрёт всю историю изменений после этого коммита 

## Ветки в git
Новая ветка создаётся с помощью команды *git branch <название ветки>* 
## Слияние веток и решение конфликтов

## Удаление веток
Удалить уже слитую ветку мы можем с помщью команды *git branch -d*. Для этого необходимо написать *git branch -d <название ветки>*

## Скачивание удалённого репозитория
Скачать удалённый репозиторий возможно с помощью команды *git clone*. Выполняется это так: в удобной Вам папке выаполните команду *git clone <адрес репозитоиия>* и у Вас появится папка, совпадающая с названием репозитория.

## Отправка изменений в удалённый репозиторий
Для отправки изменений в удалённый репозиторий используется команда *git push*. Для этого пишется в папке с репозиторием команда *git push origin <название ветки>*, чаще всего используется ветка **master**

## Pull Requests

Для принятия изменений из ветки в ветку в нашем репозитории, или из из форка удалённого репозитория в удалённый репозиторий используются Pull request'ы
