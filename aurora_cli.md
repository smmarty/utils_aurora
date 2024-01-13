#### Обновление Aurora-CLI, если уже установлена
```shell
 sudo snap refresh aurora-cli
```

#### Установка Aurora PSDK
```shell
aurora-cli psdk --install
```
Выбираем версию PSDK для установки.

#### Перезапускаем терминал
```shell
bash  
```
#### Проверка установки
```shell
aurora_psdk sdk-assistant list
```

#### Получения списка доступных версий Flutter
```shell
aurora-cli flutter --available
```

#### Установка Flutter
```shell
aurora-cli flutter --install 3.16.2
```
#### Перезапускаем терминал
```shell
bash  
```

#### Проверка установки Flutter
```shell
flutter-aurora-3.16.2 doctor
```
