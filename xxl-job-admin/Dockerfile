FROM openjdk:7-jre-slim
MAINTAINER huangyinqiang

ENV PARAMS=""
LABEL Descripttion="iioss from xxl-job-admin 2.1.0"
ENV TZ=PRC
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

ADD target/xxl-job-admin-*.jar /app.jar

ENTRYPOINT ["sh","-c","java -jar /app.jar $PARAMS"]