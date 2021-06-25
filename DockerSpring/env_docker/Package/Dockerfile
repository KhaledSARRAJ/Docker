FROM openjdk:8u292-slim

MAINTAINER Khaled <khaledinat@gmail.com>

#espace temporaire pour lui ce tmp
VOLUME /tmp  

#Ajouter ton jar qui se trouve dans le target suite a mvn clean package
ADD demoDockerAvecSpringBoot-1.0.jar app.jar

#Le port d exposition
EXPOSE 8081 

#Executer le jar: ecrire les commandes en separants par ,   
#pour de raison de security doc spring nous conseille d'ajouter -Djava.security.egd=file:/dev/./urandom  mais ca est par defaut
ENTRYPOINT ["java","-jar","-Djava.security.egd=file:/dev/./urandom","/app.jar"]