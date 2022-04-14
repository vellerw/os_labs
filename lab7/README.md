# Лабораторная работа № 7
Задание: 
* Настроить консул ( использовать уже готовую роль и инветори).
* База данных должна быть проинициализирована на выделенных дисках (в Vargrantfile они уже подключены). БД должна находить в папке /pgsql/pg_data/14. WAL архивы должны находить в папке /pgsql/pg_wal/14. В эти папки должны быть примонтированы диски /dev/sdb и /dev/sdc соответственно. 
* Диски должны быть подключены в LVM и отформатированы в файловой системе xfs.
* На серверах pg1 и pg2 настроить оркестратор репликации Patroni (пакет в архиве).
* С помощью утилиты vip-manager обеспечить настройку VIP адреса на мастер сервере. https://github.com/cybertec-postgresql/vip-manager/releases/download/v1.0.2/vip-manager-1.0.2-1.x86_64.rpm

____
* Проверяем Vagrantfile и исправляем данные, которые нам необходимы
* Запускаем Vagrantfile. После его завершения запускаем consul.play

```
vagrant up
```
```
ansible-playbook consul.play
```

* Создаем папку(roles) где будут хранится все playbooks и конифуграции для наших clients
* Запускаем playbook.yml, в котором прописано к каким hosts принадлежат папки

```
ansible-playbook playbook.yml
```
____
Заходим на один из clients:

<a href="https://ibb.co/DC5gcPt"><img src="https://i.ibb.co/DC5gcPt/2022-04-14-20-20-43-cut-photo-ru.png" alt="2022-04-14-20-20-43-cut-photo-ru" border="0"></a>
