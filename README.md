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
