# Задание
Есть: web1, web2.
* На каждый установить Nginx.
* На серверах haproxy1, haproxy2 установить и настроить  отказоустойчивую связку HAProxy+Keepalived. 
* На серверах web1, web2 Nginx должен работать по порту 8080 и отдавать кастомную страницу.
* На серверах с HAProxy ПО обеспечить балансировку нагрузки серверов web1 и web2 в режиме round-robin
* Сделать таймауты ожидания ответа web1 и web2 как можно меньше.
* Установка и настройка ПО должна быть обеспечена Ansible-сценарием.

___
## Запуск Ansible Playbook

```
vagrant up
```
```
ansible-playbook *название.yml*
```
___
## Результат web 1

работает все

<a href="https://ibb.co/cDC2CJy"><img src="https://i.ibb.co/18dRdZ0/2022-04-07-09-49-12-cut-photo-ru.png" alt="2022-04-07-09-49-12-cut-photo-ru" border="0"></a> 

выключен haproxy 1

<a href="https://ibb.co/5KRSCBc"><img src="https://i.ibb.co/kmSwzQc/2022-04-07-09-57-25-cut-photo-ru.png" alt="2022-04-07-09-57-25-cut-photo-ru" border="0"></a> 

выключен haproxy 2 

<a href="https://ibb.co/qjgY0kP"><img src="https://i.ibb.co/GpMQscb/2022-04-07-10-05-39-cut-photo-ru.png" alt="2022-04-07-10-05-39-cut-photo-ru" border="0"></a>

___
## Результат web 2

работает все

<a href="https://ibb.co/2cbpK3k"><img src="https://i.ibb.co/ZcZbTzM/2022-04-07-10-16-56-cut-photo-ru.png" alt="2022-04-07-10-16-56-cut-photo-ru" border="0"></a>

работает haproxy 1

<a href="https://ibb.co/zSLsWM9"><img src="https://i.ibb.co/4jDWwqv/2022-04-07-10-47-23-cut-photo-ru.png" alt="2022-04-07-10-47-23-cut-photo-ru" border="0"></a>

работает haproxy 2

<a href="https://ibb.co/2cbpK3k"><img src="https://i.ibb.co/ZcZbTzM/2022-04-07-10-16-56-cut-photo-ru.png" alt="2022-04-07-10-16-56-cut-photo-ru" border="0"></a>