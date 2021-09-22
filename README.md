# canal-es7

JDK：1.8版本及以上；

ElasticSearch：7.x版本；

mysql：5.7版本；

Canal.deployer：1.1.5

Canal.Adapter：1.1.5

此版本修复Load canal adapter: es7 failed问题

#修改以下配置文件即可
canal-adapter/conf/application.yml
canal-adapter/conf/es7/user_access_log.yml
canal-deployer/conf/crmeb/instance.properties


#全量数据同步
curl http://127.0.0.1:8081/etl/es7/user_access_log.yml -X POST

#参考文献
https://github.com/alibaba/canal
https://www.cnblogs.com/caoweixiong/p/11825303.html
https://zhuanlan.zhihu.com/p/270191947