#An Ambari Service for Impala


##To download the Impala service folder, run below    

clone from shuhuai007's ambari-impala-service, change centos 6 to centos 7

```
VERSION=`hdp-select status hadoop-client | sed 's/hadoop-client - \([0-9]\.[0-9]\).*/\1/'`
sudo git clone https://github.com/harryhan1989/ambari-impala-service.git /var/lib/ambari-server/resources/stacks/HDP/$VERSION/services/IMPALA        
```

##Restart Ambari
\#sandbox  
service ambari restart

\#non sandbox  
sudo service ambari-server restart