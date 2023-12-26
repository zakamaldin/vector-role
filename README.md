vector-role
=========

Роль состоит из следующих tasks:

- `Make Vector temp directory` - выполняет создане директории, куда будет скачан и извлечен пакет Vector
- `Download Vector` - выполняет скачивание пакета Vector
- `Unarchive package` - выполняет разархивирование(установку) скачанного пакета Vector в заданную директорию
- `Create Vector system user` - выполняет создание системного пользователя `vector` для запуска пакета Vector
- `Install Vector` - копирут исполняемый файл пакета Vector в директорию /usr/bin
- `Make Vector data directory` - выполняет создание директории, где будут храниться данные пакета Vector
- `Make Vector config directory` - выполняет создание директории, где будет храниться конфигурация пакета Vector
- `Configure Vector` - выполняет конфигурирование пакета Vector
- `Create Vector service` - выполняет создание сервиса в systemd
- `Reload Daemon` - выполняет перезаупск службы демона systemd, для дальнейшего запуска пакета Vector через хэндлер `Start Vector service`

Role Variables
--------------

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `vector_version` | 0.34.0 | Версия сервиса Vector, который будет скачан и установлен на целевой хост |

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: vector-role}

License
-------

MIT

Author Information
------------------

Zakamaldin Andrey
