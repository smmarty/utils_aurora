#### Установка инструментов
```shell
 sudo apt-get update
 sudo apt-get install curl git git-lfs unzip bzip2
```

#### Установка Aurora CLI
```shell
sudo snap install aurora-cli --devmode
```

#### Установка Aurora PSDK
```shell
aurora-cli psdk --install
```
#### Проверка установки
```shell
bash  
```
#### Проверка установки
```shell
aurora_psdk sdk-assistant list
```

#### Получения списка доступных версий Flutter
```shell
aurora-cli flutter --versions-available
```

#### Установка Flutter
```shell
aurora-cli flutter --install 3.16.2
```

#### Для теста скачаем для теста flutter_plugins
```shell
git clone https://gitlab.com/omprussia/flutter/flutter-plugins.git
```