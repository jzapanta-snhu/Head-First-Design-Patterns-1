
FROM openjdk:8u181-jdk

ARG JAVA_OPTS
ENV JAVA_OPTS=$JAVA_OPTS

RUN mkdir /src
RUN mkdir /app
ADD . /src

WORKDIR /src
RUN ls -al

RUN javac -d /app -verbose *.java
RUN ls -al

WORKDIR /app

RUN ls -al

ENTRYPOINT ["java","headfirst/designpatterns/strategy/MiniDuckSimulator"]