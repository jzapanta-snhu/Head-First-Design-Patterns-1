
FROM openjdk:8u181-jdk

VOLUME /tmp

RUN mkdir /app
ADD . /app

WORKDIR /app
RUN ls -al

RUN javac *.java

RUN jar cf ./duck.jar *.class

CMD ["java", "-cp", "/app/duck.jar", "headfirst.designpatterns.strategy.MiniDuckSimulator"]