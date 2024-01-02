Hа основании vjtuj проекта сделаю образ и его запушу
в контейнере. Для этого в проекта создам файл Dockerfile:

FROM openjdk
WORKDIR /app
COPY . /app
RUN javac Task1.java
CMD ["Java","Task1"]

Останавливаю проект. Захожу в терминале в корень  
проекта, где лежит Dockerfile и сейчас буду строить 
образ. Выполним команду docker build.

Docker daemon должен стянуть всё необходимое с docker hub. 
Образ готов.

Посмотреть мои образы можно через команду docker images 
в командной строке или использовать Docker Desktop. 
Находим его во вкладке Images:
