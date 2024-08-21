# modul-1.4
## Задание 1.
- https://hub.docker.com/r/andruwkakz/custom-nginx
## Задание 2.
![image](https://github.com/user-attachments/assets/74916e00-5129-41a5-b55f-6dc3979c7b41)
## Задание 3.
- ![image](https://github.com/user-attachments/assets/ee1d4d71-e85b-4567-86f9-a94b311d412f)
- ![image](https://github.com/user-attachments/assets/fba986bd-9f5d-46bb-bb86-00741bf0e7f9)
- ![image](https://github.com/user-attachments/assets/c80cb6c5-7ee3-4d9c-b7b5-64448e517c83)
Данная ситуация возникла в звязи с тем что я переназначил стандартный порт nginx с 80 на 81, а проброс портов из контейнера на хост 80:8080 соотвтетственно на 80 порту контейнера сейчас ничего нету.

- Для того что бы исправить это не удаляя контейнер нужно в линукс найти файл hostconfig.json (/var/lib/docker/containers/{id container}/) и изменить параметр биндинга контейнера с 80 на 81, если же работа проводиться в виндовс с помощью wsl, для исправления без удаления необходимо изментить тот же файл hostconfig.json находящийся по адресу \\wsl$\docker-desktop-data\data\docker\containers\{id container}\, так же в файле config.v2.json расположенному по тому же адресу в параметре ExposedPorts изменить с 80 на 81
- ![image](https://github.com/user-attachments/assets/762d5927-8fb6-4fe6-9428-4a2d249b7fa1)
- ![image](https://github.com/user-attachments/assets/97f4cb96-d42a-4c02-8845-cea5a04a15da)
## Задание 4.

## Задание 5.
1. compose.yaml - это современный версия описания, docker-compose.yaml же более старая версия и если запускать docker compose из дериктории где оба файла то запуститься более современная версия.
![image](https://github.com/user-attachments/assets/61e4aa0d-c94e-4de9-8f68-bf0c4d7328a4)
2.
![image](https://github.com/user-attachments/assets/e7c65c64-c3fc-46f2-a85d-83ffaa17bf63)
3. 
![image](https://github.com/user-attachments/assets/dde443ab-4a5e-4492-b531-e161d801a998)





