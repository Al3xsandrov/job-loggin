____
# Git
##### Установка
- Linux:
```
    $ sudo apt-get install git
```
- Mac OS:
```
    $ brew install git
```

#### Настройка
```
    $ git config --global user.name "My Name"
    $ git config --global user.email myEmail@example.com
```
#### Создание нового репозитория
```
    $ git init
```
#### Подготовка файлов и коммит
- Посмотреть информацию о текущем состоянии репозитория:
``` 
    $ git status
```
- Добавить файлы в будущий коммит:
``` 
    $ git add file.name // определенный file.name
    $ git add .         // все файлы
    $ git add -A        // также все файлы
```
- Коммит:
``` 
    $ git commit -m "Комментарий к коммиту"
```
#### Подключение к удаленному репозиторию
```
    $ git remote add origin https://github.com/...yourUrl.git
```
#### Отправка изменений на сервер
```
    $ git push origin master
```
После чего сервис может потребоваться аутентифицироваться. Вводим _Username_ и пароль.
> С августа 2021 года _Github_ отменил аутентификацию по паролю. Вместо него следует использовать Personal access tokens, который можно сгенерировать в настройках своего профиля - https://github.com/settings/tokens .
#### Получение изменений с сервера Git
```
    $ git pull origin master
```
#### Клонирование репозитория
```
    $ git clone https://github.com/...yourUrl.git