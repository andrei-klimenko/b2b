
Управление firewall для множества хостов может быть осуществлено с помощью следующих вариантов.

1. Настройка и создание security groups и access control lists для cluster или серверов через terraform

2. Конфигурация waf для alb (firewall для load balancer)

3. Если есть доступ до сервером можно использовать ansible:
  - [iptables](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/iptables_module.html)
  - [ferm](https://github.com/debops/ansible-ferm)

4. Haproxy - для перенаправление трафика через одну единственную ноду. Например, чтобы ограничить у всех остальных доступ в интернет.
