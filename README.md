ambari-kylin-service
===

## To download the Kylin service folder, run below    

HDP2.6中使用Kylin2.6.1
wget http://mirrors.tuna.tsinghua.edu.cn/apache/kylin/apache-kylin-2.6.1/apache-kylin-2.6.1-bin-hadoop3.tar.gz

```
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`
sudo git clone https://github.com/chenhai940205/ambari-kylin-service.git /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/KYLIN
```
## Restart Ambari
service ambari restart

