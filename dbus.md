[Ссылка на документацию по DBus](https://developer.auroraos.ru/doc/software_development/reference/d-bus)

[Ссылка по DBus API](https://developer.auroraos.ru/doc/4.1.0/software_development/reference/device_info)

#### Добавление поддержки Авроры
```shell
flutter create --platforms=aurora --org=com.example .
```

#### Список интерфейсов в текущей сессии
```shell
dbus-send --session           \
  --dest=org.freedesktop.DBus \
  --type=method_call          \
  --print-reply               \
  /org/freedesktop/DBus       \
  org.freedesktop.DBus.ListNames
```

#### Список интерфейсов в системе
```shell
dbus-send --system            \
   --dest=org.freedesktop.DBus \
   --type=method_call          \
   --print-reply               \
   /org/freedesktop/DBus       \
   org.freedesktop.DBus.ListNames
```
