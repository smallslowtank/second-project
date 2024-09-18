#### **Второй проект** на бесплатном курсе по основам работы с **Git**.  
[Бесплатный курс по основам Git на Яндекс Практикуме](https://start.practicum.yandex/git-basics)<br>
Установка Git и проверка версии.

```
$ sudo apt-get install git
$ git --version
```

Настройка Git. Файл конфигурации **.gitconfig**<br>
Добавить имя и почту пользователя.

```
$ git config --global user.name "user_name"
$ git config --global user.email user@email
```

Сделать папку репозиторием. Войти в папку и выполнить в ней команду.

```
$ git init
```

Разгитить папку (удалить репозиторий). В папке с репозиторием удалить скрытую папку **.git**

```
$ rm -rf .git
```

Добавление и отслеживание файла или всех файлов в репозиторий. Команды выполняются в папке с репозиторием.

```
$ git add file
$ git add --all
$ git add .
```

Проверска состояния (статуса) репозитория.

```
$ git status
```

Отправить коммит, сохранить текущую версию файлов в репозитории.

```
$ git commit -m "комментарий к коммиту"
```

Просмотр логов репозитория в полном и кратком виде.

```
$ git log
$ git log --oneline
```

Проверка ssh-ключа на GitHub.

```
$ ssh -T git@github.com
```

Связать локальный репозиторий с удалённым на GitHub.

```bash
$ git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git
```

Проверить что репозитории связаны.

```
$ git remote -v
```

Отправить изменения в удалённый репозиторий.

Первый раз выполнить команду и связать ветки.

```
$ git push -u origin main # или master
```

В следующий раз и далее.

```
$ git push
```

**Статусы файлов в репозитории:**
- untracked (не отслеживается)
- tracked (отслеживается)
- staged (подготовленный, отслеживается)
- modified (изменённый, отслеживается)

**Стили оформления коммитов:**
- Корпоративный
- Conventional Commits
- GitHub

Файл **README.md**<br>
Можно использовать язык разметки **markdown** [Шпаргалка](https://gist.github.com/fomvasss/8dd8cd7f88c67a4e3727f9d39224a84c)<br>
И формат описания схем [Mermaid](https://github.blog/developer-skills/github/include-diagrams-markdown-files-mermaid)

**Редактирование последнего коммита**<br>
Добавить файл, не менять комментарий.

```
$ git add file
$ git commit --amend --no-edit
```

Изменить комментарий.

```
$ git commit --amend -m "Новый комментарий"
```

Убрать файл из списка на коммит (после git add)

```
$ git restore --staged file
```

Убрать все файлы из списка на коммит

```
$ git restore --staged .
```

Откатиться к коммиту (коммиты после этого будут потеряны)

```
$ git reset --hard <commit_hash>
```

Откатить изменения файла, которые не попали в список на коммит и в сам коммит

```
$ git restore file
```

Сравнить последние закоммиченные версии файлов с теми, что находится в состоянии **modified**

```
$ git diff
```

Сравнить закоммиченные версии файлов с теми, что в состоянии **staged**

```
$ git diff --staged
```

Сравнить два коммита

```
$ git diff <хеш> <хеш>
```

Список игнорируемых файлов хранится в корне репозитория в файле **.gitignore**, его так же нужно коммитить, в нём можно использовать шаблоны.<br>
Просмотр игнорируемых файлов

```
$ git status --ignored
```

Клонировать на локальный компьютер репозиторий и связать его с удалённым

```
$ git clone <....>
```

Просмотр веток проекта

```
$ git branch
```

Добавить новую ветку

```bash
$ git branch <название_ветки>
```

Перейти в другую ветку

```bash
$ git checkout <название_ветки>
```

Создать ветку и сразу перейти в неё

```bash
$ git checkout -b <название_ветки>
```

Просмотр всех веток, в том числе в удалённом репозитории

```
$ git branch -a
```

Сравнить две ветки

```
$ git diff <ветка1> <ветка1>
```

Сравнить ветку с коммитом

```
$ git diff <ветка> <хеш>
```



