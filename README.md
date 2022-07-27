# Домашнее задание к занятию "08.03 Работа с Roles"

При попытке выполнить `molecule test` получил ошибку:

`TASK [roles : Upload tar.gz Elasticsearch from remote URL] *********************`

Что было ожидаемо.

Для понимания как работают `roles` в `ansible` сделал простую роль для установки [Midnight Commander](./mc/). На ней выпонил  [molecule test](./molecule.md)

Проверил, что роль отрабатывает [site.yml](site.yml)

Разобрался как работает роль [mnt-homeworks-ansible](./mnt-homeworks-ansible/). Запустил для разных ОС. 
