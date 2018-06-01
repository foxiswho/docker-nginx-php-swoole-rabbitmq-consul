# docker-nginx-php-swoole-rabbitmq-consul
docker nginx php swoole rabbitmq consul demo

更多请看
https://blog.csdn.net/fenglailea/article/details/80515310


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

# 下载docker 环境
https://github.com/foxiswho/docker-nginx-php-swoole-rabbitmq-consul
```SHELL
git clone https://github.com/foxiswho/docker-nginx-php-swoole-rabbitmq-consul.git
```
# 下载案例文件
进入上面下载的目录`wwwroot`内
```SHELL
cd wwwroot
```
然后下载 案例文件
```SHELL
git clone https://github.com/foxiswho/php-swoole-rabbitmq-consul-demo.git "dpsrc"
```
# 启动docker  compose
到根目录(有`docker-compose.yml`的那个目录),然后执行
```SHELL
docker-compose up 
```
如果你需要关闭或者删除`docker-compose up `建立的所有容器，请在`docker-compose.yml`的目录下，执行如下命令
```SHELL
docker-compose down 
```
# 启动成功后
docker compose 启动成功后，先在浏览器访问`http://localhost/demo/service_demo_mq_client/index`，有程序自动创建消息队列的交换机，队列，路由KEY等。
然后再启动如下2个DOCKER：
```SHELL
docker-nginx-php-swoole-rabbitmq-consul_phpmqsub_1
docker-nginx-php-swoole-rabbitmq-consul_phpmqsub002_1
```
为什么要其中这2个docker呢，因为在`docker  compose`创建时，消息队列里面全部是空的，没有建立测试里面的测试用的交换机，队列，路由KEY。执行一次后，就会自动创建这些



直接访问浏览器网址 即可
http://localhost/demo/service_demo_client/index
或
http://localhost/demo/service_demo_mq_client/index
