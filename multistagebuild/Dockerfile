FROM maven:3.6.3-openjdk-8
LABEL "team"="LathaMahesh"
RUN git clone 'https://github.com/spring-projects/spring-petclinic.git'
RUN cd spring-petclinic/ && maven package


FROM openjdk:8
COPY --from=packaging   /spring-petclinic/target/spring-petclinic-2.3.0.BUILD-SNAPSHOT.jar /spring-petclinic.jar
EXPOSE 8080
CMD [ "java" "-jar" ,"/spring-petclinic.jar" ]