# geckonoff_microservices
geckonoff microservices repository

ДЗ 14
В данном дз мы научились рабоать с Docker контейнерами
Создавать их удалять и тд
Научились создавать образы
Развернули тестовое приложение
В задании со * были созданы ВМ в яндекс облаке с помощью terraform 
Настроены с помощью ansible ВМ и запущен докер контейнер с приложением из образа на Docker Hub который мы создали
Для запуска сборки образа в облаке с помощью packer используйте команду
packer build -var-file=packer/variables.json  packer/docker.json
из директории docker-monolith

ДЗ 15
В данном ДЗ мы научились разбивать приложение на несколько контейнеров
Создали сеть для взаимодействия приложений
Научились пользоваться линтером
Научились оптимизировать контейнеры
Способы оптимизации:
 не использовать жирные образы - типа ubuntu
 располагать команды Dockerfile в следующием порядке
 ENV
 RUN
 COPY
 CMD

ДЗ 16
В данном ДЗ мы научились работать с сетью Docker
Создавать разные виды сети
loop
host
birdge
Научились управлять соединениями не заходя в контейнер
Посмотрели на правила iptables создаваемые для Docker контейнеров
Научились собирать docker-compose

Для задания с именами пректа необходимо задать опцию --porject-name= или просто -p
docker-compose --project-name=reddit up -d
В противном случае по умолчанию название проекта присваивается согласно названию директории откуда был произведен запуск сборки.

ДЗ monitoring-1
В данном ДЗ мы научились собирать и разворачивать систему мониторинга Prometheus
Подключили node reporter
Убелились что система мониторинга отрабатывает отсутствие любого из сервисов из которых состоит наше приложение
А так же запостили образа на docker hub

https://hub.docker.com/u/geckonoff

В задании со * для мониторинга MongoDB был использован bitnami/mongodb-exporter
https://hub.docker.com/r/bitnami/mongodb-exporter

В задании со * при мониторинге с помощью blackbox exporter использовался модуль icmp. Живость контейнеров проверяется с помощью обычного ping-а
