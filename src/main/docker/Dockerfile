FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD cls-discovery-service-0.0.1-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENV SPRING_APPLICATION_NAME=cls-discovery-service
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]