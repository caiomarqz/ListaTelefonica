FROM openjdk:11
ADD target/spring-boot-docker.jar /web/spring-boot-docker.jar
ADD target/dockscript.sh dockscript.sh
COPY ReactFrontListaTefonica-main/ /web/
EXPOSE 8080
EXPOSE 3000
RUN apt-get update -y
RUN apt-get install -y npm
WORKDIR /web
ENTRYPOINT ["sh","/dockscript.sh"]
