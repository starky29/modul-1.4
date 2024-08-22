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
- Для того что бы контейнеры с ос не гасли пришлось при запуске команды запустить команду tail -f /etc/passwd для того что бы процесс висел и не тушил контейнер
![image](https://github.com/user-attachments/assets/da15d381-a4fe-4c90-9995-d38941d60fc5)
- ![image](https://github.com/user-attachments/assets/08a2cbc7-e591-44b5-9399-4b55dd14f42e)

## Задание 5.
1. compose.yaml - это современный версия описания, docker-compose.yaml же более старая версия и если запускать docker compose из дериктории где оба файла то запуститься более современная версия.
![image](https://github.com/user-attachments/assets/61e4aa0d-c94e-4de9-8f68-bf0c4d7328a4)
2.
![image](https://github.com/user-attachments/assets/e7c65c64-c3fc-46f2-a85d-83ffaa17bf63)
3. 
![image](https://github.com/user-attachments/assets/dde443ab-4a5e-4492-b531-e161d801a998)
4. 
![image](https://github.com/user-attachments/assets/7fd8aafa-e30a-4eea-9ba5-1c6247ebe8e7)
5. 
![image](https://github.com/user-attachments/assets/69e2c555-4c10-4bf1-81e2-547e36d0707f)
6. 

![image](https://github.com/user-attachments/assets/3bcf6b39-018e-4805-a659-2717f0d95df6)

7. Суть варнинга в том, что docker compose не видит 1 из монифестов и предлагает очистить историю о нем. 
![image](https://github.com/user-attachments/assets/5c31528b-cc9c-4408-8625-4ca0a57a5086)






