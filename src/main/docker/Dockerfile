FROM frolvlad/alpine-oraclejdk8:slim
ADD cls-discovery-service-0.0.1-SNAPSHOT.jar cls-discovery-service-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /cls-discovery-service-0.0.1-SNAPSHOT.jar'
ENV JAVA_OPTS=""
ENV SPRING_APPLICATION_NAME=cls-discovery-service
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /cls-discovery-service-0.0.1-SNAPSHOT.jar" ]