# Инструкция по работе с GIT.

## git init
Команда *git init* создает git репозиторий в текущей папке. После создания репозитория появится скрытая папка .git

## git add 
Команда *git add* добавляет файл в список отслеживаемых (индексируемых) файлов для последующего коммита. Для использования необходимо написать *git init <имя файла>*

## git status

Команда необходима для просмотра состояния репозитория, изменений в файлах.

## git commit 
Команда *git commit* фиксирует / сохраненяет изменения. Для использования необходимо написать *git commit -m "<сообщение к коммиту>*

## git log
Команда *git log* взывает журнал изменений.

Чтобы посмотреть всю историю коммитов в виде графика, необходимо использовать команду *git log --graph*.

## git checkout
Команда *git checkout* необходима для переключения между версиями. Для использования необходимо написать *git checkout <номер коммита/название ветки>*

**Внимание!** для работы необходимо не только указать интересующий коммит, но и вернуться в тот, где работаем при помощи команды *git checkout master*.

## git diff
Команда *git diff* показывает разнцу между текущим файлом и сохраненным.

# Для написания заголовка в начале предложения написать #.
## Для написания подзаголовка в начале предложения написать ##.

**Для выделения текста жирным проставить ** с обеих сторон текста.**

*Для выделения курсивом проставить * с обеих сторон текста.*

## Работа с ветками GIT

## Создание ветки
Чтобы создать ветку необходимо ввести команду *git branch <branch_name>*.
Чтобы переключиться на ветку необходимо использовать команду *git checkout <branch_name>*. 
Команда *git checkout -b <branch_name>* одновременн создает и переключается на созданную ветку.

## Слияние веток
Чтобы слить изменения из одной ветки в другую необходимо использовать команду *git merge <branch_name>*, при этом курсор *HEAD* должен указывать на ту ветку, в которую сливаются изменения.

## Удаление веток
Чтобы удалить ветку, необходимо использовать команду *git branch -d<branch_name>*

## Флаги в git
Можно добавить флаги *--oneline*, *--all*, *--decorate*

## Добавление изображения
Чтобы вставить изображение в текст, необходимо сделать следующее:
![тут должна быть картинка кота](WoodyElen.jpg)

# Работа с удаленными репозиториями на github.com

## git clone 
Команда используется для копирования внешнего репозитория в локальный.
Команда *git clone* не только загружает все изменения, но и пытается слить все ветки на локальном компьютере и в удаленном репозитории.

## git pull
Команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией

## git push
Команда необходима для отправления свей версии репозитория во внешний репозиторий. При первом её использовании нужна авторизация.

## pull request
* команда для предложения изменений
* запрос на вливание изменений в репозиторий

**Как сделать *pull request*?**

1. Делаем   (ответвление) репозитория fork
2. Делаем git clone   версии репозитория СВОЕЙ
3. Создаем новую ветку и в НЕЕ вносим свои изменения
4. Фиксируем изменения (делаем коммиты)
5. Отправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку pull request