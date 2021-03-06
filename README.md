# Apache Qpid
Qpid Java offers an AMQP-fluent implementation of JMS and a message broker written in Java that stores, routes, and forwards messages using AMQP. 

## Start a Qpid instance

```sh
$ docker run --name some-qpid abh1sh3k/apache-qpid
```

## Start a Qpid instance with custom configuration file

```sh
$ docker run --name some-qpid -v $PWD/config.json:/root/config.json abh1sh3k/apache-qpid
```

## Start a Qpid instance with port map

```sh
$ docker run --name some-qpid -p 5672:5672 -p 8080:8080 abh1sh3k/apache-qpid
```

## Start a Qpid instance with persistent volume

```sh
$ docker run --name some-qpid -v $PWD/qpid-data:/root abh1sh3k/apache-qpid
```