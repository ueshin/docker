FROM ubuntu-java8

MAINTAINER Takuya UESHIN ueshin@happy-camper.st

RUN apt-get install -y git

RUN useradd -m -s /bin/bash spark

USER spark
WORKDIR /home/spark
RUN git clone https://github.com/apache/spark.git
WORKDIR /home/spark/spark
RUN sbt/sbt -Phive assembly

ENTRYPOINT ["bin/spark-shell"]
