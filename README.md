ambari-kylin-service
===

## To download the Kylin service folder, run below    

## HDP2.6与Kylin2.5.1集成使用的一版

## 下载kylin
wget https://archive.apache.org/dist/kylin/apache-kylin-2.5.1/apache-kylin-2.5.1-bin-hbase1x.tar.gz

```
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`
sudo git clone https://github.com/cas-bigdatalab/ambari-kylin-service.git /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/KYLIN
```
## Restart Ambari
\#sandbox  
service ambari restart

\#non sandbox  
sudo service ambari-server restart

## SUMMARY
![Image](../master/screenshots/kylin.png?raw=true)