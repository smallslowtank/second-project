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

