# Лабораторная работа № 4
####
Дано 3 виртуальные машины:

* rrobin
* web1
* web2

#### Задача: 
* Сервера web1, web2 должны работать по порту 8080, отдавать кастомную страницу;
* На сервере rrobin должна быть балансировка нагрузки серверов web1 и web2;
* Установка и настройка должна быть Ansible-сценарием;
* Создать playbook, где расписываем роли  web1, web2, rrobin

#### Используемые команды: 

```
vagrant up
```
> Запуск виртуальных машин и серверов

```
ansible-playbook nginx.yml
```
> Запуск самого Playbook-а

## Кастомная страница 1

<a href="https://ibb.co/SVbkcLZ"><img src="https://i.ibb.co/ssnTCBX/2022-04-04-22-48-11-cut-photo-ru.png" alt="2022-04-04-22-48-11-cut-photo-ru" border="0"></a>

## Кастомная страница 2 
<a href="https://ibb.co/rH3RpRS"><img src="https://i.ibb.co/1TMtXt5/2022-04-04-22-48-15-cut-photo-ru.png" alt="2022-04-04-22-48-15-cut-photo-ru" border="0"></a>