FROM openjdk:8
LABEL "team"="Latha Mahesh"
ARG download_location="https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"
ENV File_location= 'spring-petclinic.jar'
ADD ${download_location} ${File_location}}
EXPOSE 8080
CMD  "java" "-jar" , ${File_location}