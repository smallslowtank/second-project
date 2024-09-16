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

