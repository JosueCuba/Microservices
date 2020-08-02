FROM centos
RUN yum install -y java
ADD /out/artifacts/microservice_jar/microservice.jar app.jar
RUN sh -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]