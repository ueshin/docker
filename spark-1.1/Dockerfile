FROM ubuntu-java8

MAINTAINER Takuya UESHIN ueshin@happy-camper.st

RUN apt-get install -y git

RUN useradd -m -s /bin/bash spark

USER spark
WORKDIR /home/spark
RUN git clone -b v1.1.0-rc3 https://github.com/apache/spark.git
WORKDIR /home/spark/spark
RUN rm -rf .git
RUN sbt/sbt -Phive assembly

ENTRYPOINT bin/spark-shell
