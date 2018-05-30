# docker-nginx-php-swoole-rabbitmq-consul
docker nginx php swoole rabbitmq consul demo

未完待续

# docker rabbitmq
https://hub.docker.com/_/rabbitmq/

# 步骤

## 下载demo文件并指定目录 dpsrc
https://github.com/foxiswho/php-swoole-rabbitmq-consul-demo.git

```angular2html
cd wwwroot
git clone https://github.com/foxiswho/php-swoole-rabbitmq-consul-demo.git "dpsrc"
```

## 启动
```shell
docker-compose up 
```

## 关闭和删除
```shell
docker-compose down 
```

# 其他
## 注册中心访问
浏览器打开
```angular2html
http://localhost:8500/ui/
```

## 消息队列web 管理
```angular2html
http://localhost:15672/
```
默认用户及密码
guest
guest


# compose 配置说明
https://docs.docker.com/compose/compose-file/#context