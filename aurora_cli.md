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
aurora-cli flutter --install
```
Выбираем версию Flutter для установки

#### Перезапускаем терминал
```shell
bash  
```

#### Проверка установки Flutter
```shell
flutter-aurora-3.16.2-1 doctor
```
Если получаете ошибку о отсуттсвии embedder
<img width="623" alt="image" src="https://github.com/smmarty/utils_aurora/assets/48598325/dff15e8c-18c9-4b7f-9b99-8e8ae3fdff37">

Необходимо установить embedder вручную.
#### Проверка установки Flutter
```shell
aurora-cli embedder --install
```
Выбираете версию для установки

#### Перезапускаем терминал
```shell
bash
```

#### Проверка установки Flutter
```shell
flutter-aurora-3.16.2-1 doctor
```


