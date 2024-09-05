# FROM openjdk:8-jdk as build 

FROM openjdk:8-jdk

RUN rm -f /etc/localtime && \
  ln -sv /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
  echo "Asia/Shanghai" > /etc/timezone

ADD ./target/mango-1.0-SNAPSHOT.jar /opt/app/
CMD java $JAVA_OPTS -jar /opt/app/mango-1.0-SNAPSHOT.jar

EXPOSE 8080
