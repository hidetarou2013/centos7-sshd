# centos7-sshd

centos7-sshd

## 1.git clone

```sh
$ git clone git@github.com:hidetarou2013/centos7-sshd.git
```

## 2.docker build

```sh
$ cd centos7-sshd
$ docker build -t hidetarou2013/centos7-sshd .
$ docker build -t hidetarou2013/centos7-sshd:1.0 .
```

## 3.docker run


```sh
$ docker run --name centos7-sshd -d -p 10022:22 hidetarou2013/centos7-sshd:1.0
```

## 4.ssh

```
$ ssh developer@localhost -p 10022 -i id_rsa
```

### 4.1. connect passphrase

developer/developer

### 4.2. connect key

id_rsa

## 5.docker-enter

```
$ docker-enter centos7-sshd
```

