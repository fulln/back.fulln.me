FROM java:8
MAINTAINER : fulln <i@fulln.me>
VOLUME  /tmp
COPY api.jar  /opt/api/api.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/opt/api/api.jar"]
