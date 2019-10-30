Etcd study
===

This is a dummy study about basic operations and configs for etcd

based on:
 - [https://github.com/etcd-io/etcd/blob/master/Documentation/op-guide]
 - [https://github.com/bitnami/bitnami-docker-etcd]
 - [https://etcd.io/docs/v3.4.0/demo/]


Basic API

see more in  [https://github.com/etcd-io/etcd/blob/master/Documentation/v2/api.md]

lab:

get version
```bash
curl http://172.16.28.22:2379/version
```

set a key(message) value('hello world')
```bash
curl http://172.16.28.22:2379/v2/keys/message -XPUT -d value="Hello world"
```