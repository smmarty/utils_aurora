#### Клонируем код
```shell
https://github.com/gskinnerTeam/flutter-wonderous-app
```

#### Репозиторий плагинов
```shell
https://gitlab.com/omprussia/flutter/flutter-plugins/-/tree/master/packages?ref_type=heads
```

#### Репозиторий плагинов
```shell
https://gitlab.com/omprussia/flutter/flutter-plugins/-/tree/master/packages?ref_type=heads
```

#### Добавляем поддержку Авроры
```shell
flutter-aurora create --platforms=aurora --org=com.example .
```
#### Сборка приложения
```shell
flutter-aurora build aurora --release
```

#### Инициализируем переменную - путь к сборке 
```shell
PATH_TO_APP= 
```
#### Подпись приложения
Скачать тестовый сертификат и ключ можно на сайте.
https://developer.auroraos.ru/doc/software_development/guides/package_signing#public_certificates

После того, как скачали сертификат и ключ, ложите их в папку sign в корневой каталог пользователя. Далее подписываем приложение командой:
```shell
aurora_psdk rpmsign-external sign --key <ПУТЬ к КЛЮЧУ> --cert <ПУТЬ к СЕРТИФИКАТУ> $PATH_TO_APP
```

#### Копирование приложения в смартфон
```shell
scp $PATH_TO_APP  defaultuser@192.168.2.15:/home/defaultuser/Downloads
```

#### Подключение к смартфону
```shell
ssh defaultuser@192.168.2.15
```

#### Переход в режим ROOT 
Так, как в этом режиме вы получаете полный доступ. Будьте аккуратны, что бы не поломать смартфон.
```shell
devel-su
```
Вводим пароль который вы установили в при активации терминала

#### Установка пакета
```shell
pkcon install-local /home/defaultuser/Downloads/*.rpm -y
```

