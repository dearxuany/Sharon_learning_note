# Technology Learning Note Collection
记录项目：</br>
技术学习中产生的笔记、代码以及自己的一些想法与小总结；</br>
工作实践中部分关键代码的实现方法及相关资源整理；</br>
学习与工作中遇到的问题及其解决办法。</br>

## Elastic Stack & Kafka
#### 部署
* [elk 集群_ansible playbook 部署(1)_依赖配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(1)_%E4%BE%9D%E8%B5%96%E9%85%8D%E7%BD%AE.md)
* [elk 集群_ansible playbook 部署(2)_filebeat 文本收集](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(2)_filebeat.md#elk-%E9%9B%86%E7%BE%A4_ansible-playbook-%E9%83%A8%E7%BD%B22_filebeat)
* [elk 集群_ansible playbook 部署(3)_kafka 消息队列](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(3)_kafka%20%E6%B6%88%E6%81%AF%E9%98%9F%E5%88%97.md)
* [elk 集群_ansible playbook 部署(4)_logstash 过滤分析](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(4)_logstash.md)
* [elk 集群_ansible playbook 部署(5)_elasticsearch 集群](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(5)_elasticsearch%20%E9%9B%86%E7%BE%A4.md)
* [elk 集群_ansible playbook 部署(6)_kibana 可视化](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(6)_kibana%20%E5%8F%AF%E8%A7%86%E5%8C%96.md)
* [elk 集群_ansible playbook 部署(7)_kafka SSL 加密传输](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(7)_kafka%20SSL%20%E5%8A%A0%E5%AF%86%E4%BC%A0%E8%BE%93.md)
* [elk 集群_ansible playbook 部署(8)_xpack 用户认证配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E9%9B%86%E7%BE%A4_ansible%20playbook%20%E9%83%A8%E7%BD%B2(8)_xpack%20%E7%94%A8%E6%88%B7%E8%AE%A4%E8%AF%81%E9%85%8D%E7%BD%AE.md)
#### 使用
* [elk 日志分析_nginx_logstash grok & filter](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E6%97%A5%E5%BF%97%E5%88%86%E6%9E%90_nginx_logstash%20grok%20&%20filter.md)
* [elk 日志分析_ java logback json 业务日志_logstash filter](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/elk%20%E6%97%A5%E5%BF%97%E5%88%86%E6%9E%90_%20java%20logback%20json%20%E4%B8%9A%E5%8A%A1%E6%97%A5%E5%BF%97_logstash%20filter.md)
* [es 插件_Elasticsearch 7.1.1 安装 pinyin 分词器插件](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E6%8F%92%E4%BB%B6_Elasticsearch%207.1.1%20%E5%AE%89%E8%A3%85%20pinyin%20%E5%88%86%E8%AF%8D%E5%99%A8%E6%8F%92%E4%BB%B6.md)
* [es 插件_ ik 中文分词器、自定义词典](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E6%8F%92%E4%BB%B6_%20ik%20%E4%B8%AD%E6%96%87%E5%88%86%E8%AF%8D%E5%99%A8%E3%80%81%E8%87%AA%E5%AE%9A%E4%B9%89%E8%AF%8D%E5%85%B8.md)
* [es 集群节点滚动更新](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E9%9B%86%E7%BE%A4%E8%8A%82%E7%82%B9%E6%BB%9A%E5%8A%A8%E6%9B%B4%E6%96%B0.md)
#### 优化
* [es 集群优化_elasticsearch 节点重启后报 master not discovered or elected yet 无法选举 master 问题解决](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E9%9B%86%E7%BE%A4%E4%BC%98%E5%8C%96_elasticsearch%20%E8%8A%82%E7%82%B9%E9%87%8D%E5%90%AF%E5%90%8E%E6%8A%A5%20master%20not%20discovered%20or%20elected%20yet%20%E6%97%A0%E6%B3%95%E9%80%89%E4%B8%BE%20master%20%E9%97%AE%E9%A2%98%E8%A7%A3%E5%86%B3.md)
* [es 集群优化_程序无法在 es 集群自动创建 index 问题解决](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E9%9B%86%E7%BE%A4%E4%BC%98%E5%8C%96_%E7%A8%8B%E5%BA%8F%E6%97%A0%E6%B3%95%E5%9C%A8%20es%20%E9%9B%86%E7%BE%A4%E8%87%AA%E5%8A%A8%E5%88%9B%E5%BB%BA%20index%20%E9%97%AE%E9%A2%98%E8%A7%A3%E5%86%B3.md)
* [es 集群优化_设置 fielddata 缓存自动清理](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E9%9B%86%E7%BE%A4%E4%BC%98%E5%8C%96_%E8%AE%BE%E7%BD%AE%20fielddata%20%E7%BC%93%E5%AD%98%E8%87%AA%E5%8A%A8%E6%B8%85%E7%90%86.md)
* [es 集群优化_es 集群磁盘使用量达 95% 或单节点分片数达 1000 致 index 被设只读锁数据无法写入](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/%20es%20%E9%9B%86%E7%BE%A4%E4%BC%98%E5%8C%96_es%20%E9%9B%86%E7%BE%A4%E7%A3%81%E7%9B%98%E4%BD%BF%E7%94%A8%E9%87%8F%E8%BE%BE%2095%25%20%E6%88%96%E5%8D%95%E8%8A%82%E7%82%B9%E5%88%86%E7%89%87%E6%95%B0%E8%BE%BE%201000%20%E8%87%B4%20index%20%E8%A2%AB%E8%AE%BE%E5%8F%AA%E8%AF%BB%E9%94%81%E6%95%B0%E6%8D%AE%E6%97%A0%E6%B3%95%E5%86%99%E5%85%A5.md)
* [es 集群优化_磁盘水印低 Low disk watermark 导致集群节点分片分配不均匀问题解决](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E9%9B%86%E7%BE%A4%E4%BC%98%E5%8C%96_%E7%A3%81%E7%9B%98%E6%B0%B4%E5%8D%B0%E4%BD%8E%20Low%20disk%20watermark%20%E5%AF%BC%E8%87%B4%E9%9B%86%E7%BE%A4%E8%8A%82%E7%82%B9%E5%88%86%E7%89%87%E5%88%86%E9%85%8D%E4%B8%8D%E5%9D%87%E5%8C%80%E9%97%AE%E9%A2%98%E8%A7%A3%E5%86%B3.md)

#### 数据迁移同步
* [es 数据迁移_elasticsearch-dump 全量迁移 es 数据 ](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/elk_note/es%20%E6%95%B0%E6%8D%AE%E8%BF%81%E7%A7%BB_elasticsearch-dump%20%E5%85%A8%E9%87%8F%E8%BF%81%E7%A7%BB%20es%20%E6%95%B0%E6%8D%AE.md)
* [es 数据同步_canal 通过 mysql binlog 实时增量同步 mysql 数据到 elasticsearch](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/canal/canal%20%E9%80%9A%E8%BF%87%20mysql%20binlog%20%E5%A2%9E%E9%87%8F%E5%90%8C%E6%AD%A5%20mysql%20%E6%95%B0%E6%8D%AE%E5%88%B0%20elasticsearch.md)

## docker & kubernetes
* [docker、docker-compose 安装、镜像源修改](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/docker_note/docker%E3%80%81docker-compose%20%E5%AE%89%E8%A3%85%E3%80%81%E9%95%9C%E5%83%8F%E6%BA%90%E4%BF%AE%E6%94%B9.md)
* [docker 使用阿里云容器镜像仓库](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/docker_note/docker%20%E4%BD%BF%E7%94%A8%E9%98%BF%E9%87%8C%E4%BA%91%E5%AE%B9%E5%99%A8%E9%95%9C%E5%83%8F%E4%BB%93%E5%BA%93.md)
* [docker 常用命令、dockerfile_python flask example](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/docker_note/docker%20%E5%B8%B8%E7%94%A8%E5%91%BD%E4%BB%A4%E3%80%81dockerfile_python%20flask%20example.md)
* [docker-compose 部署 sentry 多语言错误跟踪工具](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/docker_note/docker-compose%20%E9%83%A8%E7%BD%B2%20sentry%20%E5%A4%9A%E8%AF%AD%E8%A8%80%E9%94%99%E8%AF%AF%E8%B7%9F%E8%B8%AA%E5%B7%A5%E5%85%B7.md)
* [NVIDIA GPU 算法专用容器 nvidia-docker 部署](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/docker_note/NVIDIA%20GPU%20%E7%AE%97%E6%B3%95%E4%B8%93%E7%94%A8%E5%AE%B9%E5%99%A8%20nvidia-docker%20%E9%83%A8%E7%BD%B2.md)

* [Kubernetes In Docker Kind 部署使用](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/k8s_note/Kubernetes%20In%20Docker%20Kind%20%E9%83%A8%E7%BD%B2%E4%BD%BF%E7%94%A8.md)
* [Kubernetes helm 部署使用](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/k8s_note/k8s%20helm%20%E9%83%A8%E7%BD%B2%E4%BD%BF%E7%94%A8.md)
* [k8s ImagePullSecrets 设置使用阿里云私有镜像仓库](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/k8s_note/k8s%20%20ImagePullSecrets%20%E8%AE%BE%E7%BD%AE%E4%BD%BF%E7%94%A8%E9%98%BF%E9%87%8C%E4%BA%91%E7%A7%81%E6%9C%89%E9%95%9C%E5%83%8F%E4%BB%93%E5%BA%93.md)
* [k8s 集群新增 gpu 节点并基于 NodeLabel 通过 nodeSelector 调度部署应用](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/k8s_note/k8s%20%E9%9B%86%E7%BE%A4%E6%96%B0%E5%A2%9E%20gpu%20%E8%8A%82%E7%82%B9%E5%B9%B6%E5%9F%BA%E4%BA%8E%20NodeLabel%20%E9%80%9A%E8%BF%87%20nodeSelector%20%E8%B0%83%E5%BA%A6%E9%83%A8%E7%BD%B2%E5%BA%94%E7%94%A8.md)

## Server
### Nginx
* [Nginx 两次跳转反代静态文件、后端服务、域名配置（公网访问办公网内服务）](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E4%B8%A4%E6%AC%A1%E8%B7%B3%E8%BD%AC%E5%8F%8D%E4%BB%A3%E9%9D%99%E6%80%81%E6%96%87%E4%BB%B6%E3%80%81%E5%90%8E%E7%AB%AF%E6%9C%8D%E5%8A%A1%E3%80%81%E5%9F%9F%E5%90%8D%E9%85%8D%E7%BD%AE%EF%BC%88%E5%85%AC%E7%BD%91%E8%AE%BF%E9%97%AE%E5%8A%9E%E5%85%AC%E7%BD%91%E5%86%85%E6%9C%8D%E5%8A%A1%EF%BC%89.md)
* [Linux(ubuntu)-Nginx-MySQL-PHP 架构 apt-get 安装配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Linux%20Nginx%20MySQL%20PHP%20%E5%AE%89%E8%A3%85%E9%85%8D%E7%BD%AE.MD)
* [Linux(CentOS7)-Nginx-MariaDB-PHP 架构 源码安装及配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Linux(CentOS7)-Nginx-MariaDB-PHP%20%E6%9E%B6%E6%9E%84%E6%BA%90%E7%A0%81%E5%AE%89%E8%A3%85%E5%8F%8A%E9%85%8D%E7%BD%AE.MD)</br>
* [Nginx 原理与特性](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E5%8E%9F%E7%90%86%E4%B8%8E%E7%89%B9%E6%80%A7.md)
* [Nginx 日志文件与切分备份](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E6%97%A5%E5%BF%97%E6%96%87%E4%BB%B6%E4%B8%8E%E5%88%87%E5%88%86%E5%A4%87%E4%BB%BD.md)
* [Nginx 性能优化](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96.md)
* [Nginx 流量及并发连接数限制](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E6%B5%81%E9%87%8F%E5%8F%8A%E5%B9%B6%E5%8F%91%E8%BF%9E%E6%8E%A5%E6%95%B0%E9%99%90%E5%88%B6%20.md)
* [Nginx 访问控制及 DDOS 预防](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E8%AE%BF%E9%97%AE%E6%8E%A7%E5%88%B6%E5%8F%8A%20DDOS%20%E9%A2%84%E9%98%B2.md)
* [Nginx 日志显示真实IP](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E6%97%A5%E5%BF%97%E6%98%BE%E7%A4%BA%E7%9C%9F%E5%AE%9EIP.md)
* [Nginx 动态加载模块](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/server_note/Nginx_note/Nginx%20%E5%8A%A8%E6%80%81%E5%8A%A0%E8%BD%BD%E6%A8%A1%E5%9D%97.md)


## APM
### Apache SkyWalking
* [Apache SkyWalking 分布式应用系统 apm 服务端部署](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/apm_note/skywalking_note/Apache%20SkyWalking%20%E5%88%86%E5%B8%83%E5%BC%8F%E5%BA%94%E7%94%A8%E7%B3%BB%E7%BB%9F%20apm%20%E6%9C%8D%E5%8A%A1%E7%AB%AF%E9%83%A8%E7%BD%B2.md)
* [Apache SkyWalking 客户端 java-agent 接入 jar、jetty、tomcat](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/apm_note/skywalking_note/Apache%20SkyWalking%20%E5%AE%A2%E6%88%B7%E7%AB%AF%20java-agent%20%E6%8E%A5%E5%85%A5.md)


## JAVA
* [JVM 性能 jstack 排查 java 进程 CPU 占用率高](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/java_note/java%20%E8%BF%9B%E7%A8%8B%20CPU%20%E4%BD%BF%E7%94%A8%E7%8E%87%E9%AB%98%20jstack%20%E6%8E%92%E6%9F%A5%E6%96%B9%E6%B3%95.md)
* [JVM 性能 jmap 生成 dump 文件排查 java 进程内存使用率高](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/java_note/java%20%E8%BF%9B%E7%A8%8B%E5%86%85%E5%AD%98%E4%BD%BF%E7%94%A8%E7%8E%87%E9%AB%98%20jmap%20%E6%8E%92%E6%9F%A5%E6%96%B9%E6%B3%95.md)

## Python
### Python3 基础
* [Python 基础语法](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%9F%BA%E7%A1%80%E8%AF%AD%E6%B3%95.MD)
* [Python 解释器](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E8%A7%A3%E9%87%8A%E5%99%A8.MD)
* [Python 序列：序列类型、通用基本操作](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%BA%8F%E5%88%97%EF%BC%9A%E5%BA%8F%E5%88%97%E7%B1%BB%E5%9E%8B%E3%80%81%E9%80%9A%E7%94%A8%E5%9F%BA%E6%9C%AC%E6%93%8D%E4%BD%9C.MD)
* [Python 序列：列表 list](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%BA%8F%E5%88%97%EF%BC%9A%E5%88%97%E8%A1%A8.MD)
* [Python 序列：元组 tuple](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%BA%8F%E5%88%97%EF%BC%9A%E5%85%83%E7%BB%84.MD)
* [Python 序列：字符串 string](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%BA%8F%E5%88%97%EF%BC%9A%E5%AD%97%E7%AC%A6%E4%B8%B2.MD)
* [Python 映射：字典 dictionary](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E6%98%A0%E5%B0%84%EF%BC%9A%E5%AD%97%E5%85%B8.MD)
* [Python 语句：赋值、条件、循环及其他语句](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E8%AF%AD%E5%8F%A5%EF%BC%9A%E8%B5%8B%E5%80%BC%E3%80%81%E6%9D%A1%E4%BB%B6%E3%80%81%E5%BE%AA%E7%8E%AF%E5%8F%8A%E5%85%B6%E4%BB%96%E8%AF%AD%E5%8F%A5.MD)
* [Python 迭代与推导](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E8%BF%AD%E4%BB%A3%E4%B8%8E%E6%8E%A8%E5%AF%BC.MD)
* [Python 函数](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%87%BD%E6%95%B0.MD)
* [Python 面向对象：类、实例、属性、方法](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%EF%BC%9A%E7%B1%BB%E3%80%81%E5%AE%9E%E4%BE%8B%E3%80%81%E5%B1%9E%E6%80%A7%E3%80%81%E6%96%B9%E6%B3%95.MD)
* [Python 错误和异常](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%94%99%E8%AF%AF%E3%80%81%E5%BC%82%E5%B8%B8%E5%8F%8A%E5%85%B6%E5%A4%84%E7%90%86.MD)
* [Python 面向对象：魔法方法 Special method、特性 property、迭代器 iterator](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%EF%BC%9ASpecial%20method%20%E9%AD%94%E6%B3%95%E6%96%B9%E6%B3%95%E3%80%81property%E7%89%B9%E6%80%A7%E3%80%81iterator%20%E8%BF%AD%E4%BB%A3%E5%99%A8.MD)
* [Python \*.py直接执行和导入解释器执行的传参问题](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20*.py%E7%9B%B4%E6%8E%A5%E6%89%A7%E8%A1%8C%E5%92%8C%E5%AF%BC%E5%85%A5%E8%A7%A3%E9%87%8A%E5%99%A8%E6%89%A7%E8%A1%8C%E7%9A%84%E4%BC%A0%E5%8F%82%E9%97%AE%E9%A2%98.md)

### Python3 模块
#### 标准库
* [Python 模块](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E6%A8%A1%E5%9D%97.MD)
* [Python 集合 set、堆 heapq、双端队列 deque、队列 queue ](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%9B%86%E5%90%88%E3%80%81%E5%A0%86%E3%80%81%E5%8F%8C%E7%AB%AF%E9%98%9F%E5%88%97%E3%80%81%E9%98%9F%E5%88%97.MD)
* [Python 日期与时间 time](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E6%97%A5%E6%9C%9F%E4%B8%8E%E6%97%B6%E9%97%B4.MD)
* [Python 随机与统计 random](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%9A%8F%E6%9C%BA%E4%B8%8E%E7%BB%9F%E8%AE%A1.MD)
* [Python 原始类与 JSON 对象转换](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E5%8E%9F%E5%A7%8B%E7%B1%BB%E4%B8%8EJSON%E5%AF%B9%E8%B1%A1%E8%BD%AC%E6%8D%A2.MD)
* [Python 正则表达式 re](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E6%AD%A3%E5%88%99%E8%A1%A8%E8%BE%BE%E5%BC%8F%20re.MD)
* [Python IO编程：文件 fileinput](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20IO%E7%BC%96%E7%A8%8B%EF%BC%9A%E6%96%87%E4%BB%B6.MD)
#### 第三方库
* [Python 通过 psutil 对 linux 进行监控](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%80%9A%E8%BF%87%20psutil%20%E5%AF%B9%20linux%20%E8%BF%9B%E8%A1%8C%E7%9B%91%E6%8E%A7.md)
* [Python 通过 yagmail 发送邮件](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E9%80%9A%E8%BF%87%20yagmail%20%E5%8F%91%E9%80%81%E9%82%AE%E4%BB%B6.MD)

### Python3 web
* [Python 使用CGI创建动态网页 cgi、cgitb](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E4%BD%BF%E7%94%A8CGI%E5%88%9B%E5%BB%BA%E5%8A%A8%E6%80%81%E7%BD%91%E9%A1%B5%20cgi%E3%80%81cgitb.MD)

### Python3 工具
* [Python 程序打包 Setuptools](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E7%A8%8B%E5%BA%8F%E6%89%93%E5%8C%85%20Setuptools.MD)
* [Python 虚拟python环境 virtualenv](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E8%99%9A%E6%8B%9Fpython%E7%8E%AF%E5%A2%83%20virtualenv.MD)
* [Python linux交互式监控工具 glances](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20linux%E4%BA%A4%E4%BA%92%E5%BC%8F%E7%9B%91%E6%8E%A7%E5%B7%A5%E5%85%B7%20glances.MD)

### Python3 算法
* [Python 算法：二分法查找、选择排序、快速排序](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E7%AE%97%E6%B3%95%EF%BC%9A%E4%BA%8C%E5%88%86%E6%B3%95%E6%9F%A5%E6%89%BE%E3%80%81%E9%80%89%E6%8B%A9%E6%8E%92%E5%BA%8F%E3%80%81%E5%BF%AB%E9%80%9F%E6%8E%92%E5%BA%8F.MD)
* [Python 算法：广度优先算法（路径最短）、狄克斯特拉算法（花销最少）](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/python_note/Python%20%E7%AE%97%E6%B3%95%EF%BC%9A%E5%B9%BF%E5%BA%A6%E4%BC%98%E5%85%88%E7%AE%97%E6%B3%95%E3%80%81%E7%8B%84%E5%85%8B%E6%96%AF%E7%89%B9%E6%8B%89%E7%AE%97%E6%B3%95%20.MD)


## Databases
### 数据库基础
* [RDBMS 与 NoSQL 的对比(CAP理论)](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/database_note/database%20RDBMS%E4%B8%8ENoSQL%E7%9A%84%E5%AF%B9%E6%AF%94.MD)
* [SQL 语句](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/database_note/database%20SQL%E8%AF%AD%E5%8F%A5.MD)
### MySQL
* [python3 连接并操作 MySQL(MariaDB)](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/database_note/database%20python3%E8%BF%9E%E6%8E%A5%E5%B9%B6%E6%93%8D%E4%BD%9CMySQL(MariaDB).MD)
* [MySQL 数据类型优化](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/database_note/database%20MySQL%20%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B%E4%BC%98%E5%8C%96.md)
* [MySQL InnoDB锁机制](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/database_note/database%20MySQL%20InnoDB%E9%94%81%E6%9C%BA%E5%88%B6.md)



## Linux
### Linux 相关知识
* [Linux 常用命令(无格式)](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20command%20%26%20SHELL%20collection)
* [Linux 目录结构](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E7%9B%AE%E5%BD%95%E7%BB%93%E6%9E%84.md)
* [Linux 文件目录命名规则](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%96%87%E4%BB%B6%E5%90%8D%E5%91%BD%E5%90%8D%E8%A7%84%E5%88%99.MD)
* [Linux 文件搜索 whereis、locate、which、find](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%96%87%E4%BB%B6%E6%90%9C%E7%B4%A2%20whereis%E3%80%81locate%E3%80%81which%E3%80%81find.md)
* [Linux 打包压缩和解压 tar](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%89%93%E5%8C%85%E5%8E%8B%E7%BC%A9%E5%91%BD%E4%BB%A4%20tar.md)
* [Linux 用户及文件权限管理](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E7%94%A8%E6%88%B7%E5%8F%8A%E6%96%87%E4%BB%B6%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86.md)
* [Linux 特殊权限管理 ACL、SUID、SGID、Sticky BIT](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E7%89%B9%E6%AE%8A%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86.md)
* [Linux 系统性能监控常用命令](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E7%B3%BB%E7%BB%9F%E6%80%A7%E8%83%BD%E7%9B%91%E6%8E%A7.md)


### Linux 设备与文件系统
* [Linux 删除多余无用分区 （命令 df lsblk fdisk）](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%88%A0%E9%99%A4%E5%A4%9A%E4%BD%99%E6%97%A0%E7%94%A8%E5%88%86%E5%8C%BA.MD)
* [Linux 文件系统根目录所在磁盘扩容 LVM](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%96%87%E4%BB%B6%E7%B3%BB%E7%BB%9F%E6%A0%B9%E7%9B%AE%E5%BD%95%E6%89%80%E5%9C%A8%E7%A3%81%E7%9B%98%E6%89%A9%E5%AE%B9.MD)

### Linux 进程与服务
* [Linux 内核、进程、线程 （命令 ps top kill）](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%86%85%E6%A0%B8%E3%80%81%E8%BF%9B%E7%A8%8B%E3%80%81%E7%BA%BF%E7%A8%8B.MD)
* [Linux IO模型：同步、异步、阻塞、非阻塞](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20IO%E6%A8%A1%E5%9E%8B%EF%BC%9A%E5%90%8C%E6%AD%A5%E3%80%81%E5%BC%82%E6%AD%A5%E3%80%81%E9%98%BB%E5%A1%9E%E3%80%81%E9%9D%9E%E9%98%BB%E5%A1%9E.MD)
* [Linux daemons 启动与管理 init、systemd](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20daemons%20%E5%90%AF%E5%8A%A8%E4%B8%8E%E7%AE%A1%E7%90%86%20init%E3%80%81systemd%20.MD)
* [Linux 端口与网络服务管理](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E7%AB%AF%E5%8F%A3%E4%B8%8E%E7%BD%91%E7%BB%9C%E6%9C%8D%E5%8A%A1%E7%AE%A1%E7%90%86.md)
* [Linux 日志系统 rsyslog logrotate systemd-journal logwatch](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%97%A5%E5%BF%97%E7%B3%BB%E7%BB%9F%20rsyslog%20logrotate%20systemd-journal%20logwatch.md)
* [Linux 时间同步 NTP](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E6%97%B6%E9%97%B4%E5%90%8C%E6%AD%A5.MD)
* [Linux 例行性工作 crontab](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E4%BE%8B%E8%A1%8C%E6%80%A7%E5%B7%A5%E4%BD%9C.MD)
* [Linux 进程后台运行 nohup](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E8%BF%9B%E7%A8%8B%E5%90%8E%E5%8F%B0%E8%BF%90%E8%A1%8C%20nohup.md)

### Linux 软件安装
#### 数据库
* [Linux yum安装配置 MySQL（MariaDB）](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%AE%89%E8%A3%85%E9%85%8D%E7%BD%AEMySQL%EF%BC%88MariaDB%EF%BC%89.MD)
* [Linux 源码安装 MongoDB](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%AE%89%E8%A3%85MongoDB.MD)
#### 编程语言
* [Linux 源码安装 python3](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%AE%89%E8%A3%85Python%203.MD)
* [Linux CentOS7 在 python2、python3 共存状态下安装 pip2 和 pip3](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20CentOS7%20%E5%9C%A8python2%E3%80%81python3%E5%85%B1%E5%AD%98%E4%B8%8B%E5%AE%89%E8%A3%85pip2%E5%92%8Cpip3.MD)
* [Linux 源码安装 Node.js](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20%E5%AE%89%E8%A3%85%E9%85%8D%E7%BD%AENode.js%20.MD)

### Linux 相关工具
* [Linux win使用putty通过ssh传文件](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/linux_note/Linux%20win%E4%BD%BF%E7%94%A8putty%E9%80%9A%E8%BF%87ssh%E4%BC%A0%E6%96%87%E4%BB%B6.md)
* [Linux git 配置与使用](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/github_note/git%20%E9%85%8D%E7%BD%AE%E4%B8%8E%E4%BD%BF%E7%94%A8.md)


## shell
* [shell linux 默认shell bash](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20linux%E9%BB%98%E8%AE%A4shell%20bash.MD)
* [shell 变量功能](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E5%8F%98%E9%87%8F%E5%8A%9F%E8%83%BD.MD)
* [shell 特殊字符、数据流重定向](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E7%89%B9%E6%AE%8A%E5%AD%97%E7%AC%A6%E3%80%81%E6%95%B0%E6%8D%AE%E6%B5%81%E9%87%8D%E5%AE%9A%E5%90%91.MD)
* [shell 正则表达式](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E6%AD%A3%E5%88%99%E8%A1%A8%E8%BE%BE%E5%BC%8F.MD)
* [shell 管道命令](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E7%AE%A1%E9%81%93%E5%91%BD%E4%BB%A4.MD)
* [shell script 逻辑判断](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E9%80%BB%E8%BE%91%E5%88%A4%E6%96%AD.MD)
* [shell script 变量、函数、循环、追踪调试](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/shell_note/shell%20%E5%8F%98%E9%87%8F%E3%80%81%E5%87%BD%E6%95%B0%E3%80%81%E5%BE%AA%E7%8E%AF%E3%80%81%E8%BF%BD%E8%B8%AA%E8%B0%83%E8%AF%95.MD)




## VMware
### VMware 相关操作
* [VMware 删除旧快照](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/VMware_note/VMware%20%E5%88%A0%E9%99%A4%E6%97%A7%E7%9A%84%E5%BF%AB%E7%85%A7.MD)
* [VMware 合并多个 vmdk](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/VMware_note/VMware%20%E5%90%88%E5%B9%B6%E5%A4%9A%E4%B8%AAvmdk.MD)
* [VMware CentOS7虚拟机 网络配置 NAT](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/VMware_note/VMware%20CentOS7%E8%99%9A%E6%8B%9F%E6%9C%BA%20%E7%BD%91%E7%BB%9C%E9%85%8D%E7%BD%AE.MD)
* [VMware 虚拟机扩容](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/VMware_note/VMware%20%E8%99%9A%E6%8B%9F%E6%9C%BA%E6%89%A9%E5%AE%B9.MD)
* [VMware 物理机磁盘空间不足问题解决](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/VMware_note/VMware%20%E7%89%A9%E7%90%86%E6%9C%BA%E7%A3%81%E7%9B%98%E7%A9%BA%E9%97%B4%E4%B8%8D%E8%B6%B3%E7%9A%84%E9%97%AE%E9%A2%98%E8%A7%A3%E5%86%B3.MD)

## Network
### Cisco Certified Network Associate
思科认证 网络工程师 CCNA  Score: 986/1000
[ Cisco Certified Network Associate Routing and Switching](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/note_images/Networking_note_images/ccna_11105536_certificate.png)
### 思科网络硬件配置
* [路由选择：开放最短路径优先 OSPF 原理与配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/network_note/Network%20%E5%BC%80%E6%94%BE%E6%9C%80%E7%9F%AD%E8%B7%AF%E5%BE%84%E4%BC%98%E5%85%88%20OSPF.md)
* [动态主机配置协议 DHCP 原理及配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/network_note/Network%20%E5%8A%A8%E6%80%81%E4%B8%BB%E6%9C%BA%E9%85%8D%E7%BD%AE%E5%8D%8F%E8%AE%AE%20DHCP.md)
* [超文本传输协议 http 与 DNS server 原理及配置](https://github.com/dearxuany/Sharon_Technology_learning_note/blob/master/network_note/Network%20%E8%B6%85%E6%96%87%E6%9C%AC%E4%BC%A0%E8%BE%93%E5%8D%8F%E8%AE%AE%20http%20.md)
