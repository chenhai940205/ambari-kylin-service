ambari-kylin-service
===

## To download the Kylin service folder, run below    

HDP2.6中使用Kylin2.5.1
wget https://archive.apache.org/dist/kylin/apache-kylin-2.5.1/apache-kylin-2.5.1-bin-hbase1x.tar.gz

```
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`
sudo git clone https://github.com/ZZZKROSS/ambari-kylin-service.git /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/KYLIN
```
## Restart Ambari
service ambari restart

