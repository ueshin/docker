# docker

Provides some Dockerfiles.

## ubuntu-java8

Installed Java8 on ubuntu base image.

### build

```bash
docker build -t ubuntu-java8 ubuntu-java8
```

## spark

Built Apache Spark on ubuntu-java8.

### build

```bash
docker build -t spark spark
```

Build ubuntu-java8 in advance.

## spark-1.0

Build Apache Spark 1.0.x on ubuntu-java8.

### build

```bash
docker build -t spark:1.0.2 spark-1.0
```

Build ubuntu-java8 in advance.
