# docker-nginx-php-swoole-rabbitmq-consul
docker nginx php swoole rabbitmq consul demo

未完待续

# docker rabbitmq
https://hub.docker.com/_/rabbitmq/

# 步骤
## 创建网络
```angular2html
docker network create -d macvlan  --subnet=172.172.0.0/19 --gateway=172.172.0.1 -o parent=eth0 macvlan
```

## 启动
```shell
docker-compose up 
```

## 关闭和删除
```shell
docker-compose down 
```


https://docs.docker.com/compose/compose-file/#context