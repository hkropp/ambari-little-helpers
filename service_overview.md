<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Service: ACCUMULO](#service-accumulo)
  - [MASTER](#master)
  - [SLAVE](#slave)
  - [CLIENT](#client)
- [Service: AMBARI_METRICS](#service-ambari_metrics)
  - [MASTER](#master-1)
  - [SLAVE](#slave-1)
- [Service: FALCON](#service-falcon)
  - [MASTER](#master-2)
  - [CLIENT](#client-1)
- [Service: FLUME](#service-flume)
  - [SLAVE](#slave-2)
- [Service: GANGLIA](#service-ganglia)
  - [MASTER](#master-3)
  - [SLAVE](#slave-3)
- [Service: HBASE](#service-hbase)
  - [MASTER](#master-4)
  - [SLAVE](#slave-4)
  - [CLIENT](#client-2)
- [Service: HDFS](#service-hdfs)
  - [MASTER](#master-5)
  - [SLAVE](#slave-5)
  - [CLIENT](#client-3)
- [Service: HIVE](#service-hive)
  - [MASTER](#master-6)
  - [CLIENT](#client-4)
- [Service: KAFKA](#service-kafka)
  - [MASTER](#master-7)
- [Service: KERBEROS](#service-kerberos)
  - [MASTER](#master-8)
  - [CLIENT](#client-5)
- [Service: KNOX](#service-knox)
  - [MASTER](#master-9)
- [Service: MAHOUT](#service-mahout)
  - [CLIENT](#client-6)
- [Service: MAPREDUCE2 (Part of YARN service)](#service-mapreduce2-part-of-yarn-service)
  - [MASTER](#master-10)
  - [CLIENT](#client-7)
- [Service: NAGIOS](#service-nagios)
- [Service: OOZIE](#service-oozie)
  - [MASTER](#master-11)
  - [CLIENT](#client-8)
- [Service: PIG](#service-pig)
  - [CLIENT](#client-9)
- [Service: RANGER](#service-ranger)
  - [MASTER](#master-12)
- [Service: RANGER_KMS](#service-ranger_kms)
  - [MASTER](#master-13)
- [Service: SLIDER](#service-slider)
  - [CLIENT](#client-10)
- [Service: SPARK](#service-spark)
  - [MASTER](#master-14)
  - [CLIENT](#client-11)
- [Service: SQOOP](#service-sqoop)
  - [CLIENT](#client-12)
- [Service: STORM](#service-storm)
  - [MASTER](#master-15)
  - [SLAVE](#slave-6)
- [Service: TEZ](#service-tez)
  - [CLIENT](#client-13)
- [Service: YARN](#service-yarn)
  - [MASTER](#master-16)
  - [SLAVE](#slave-7)
  - [CLIENT](#client-14)
- [Service: ZOOKEEPER](#service-zookeeper)
  - [MASTER](#master-17)
  - [CLIENT](#client-15)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Service: ACCUMULO
### MASTER
* ACCUMULO_MASTER (1+)
* ACCUMULO_MONITOR (1+)
* ACCUMULO_GC (1+)
* ACCUMULO_TRACER (1+)

### SLAVE
* ACCUMULO_TSERVER (1+)

### CLIENT
* ACCUMULO_CLIENT (1+)


## Service: AMBARI_METRICS
### MASTER
* METRICS_COLLECTOR (1)

### SLAVE
* METRICS_MONITOR (ALL)


## Service: FALCON
### MASTER
* FALCON_SERVER (1)

### CLIENT
* FALCON_CLIENT (1+)


## Service: FLUME
### SLAVE
* FLUME_HANDLER (1+)


## Service: GANGLIA
### MASTER
* GANGLIA_SERVER (1)

### SLAVE
* GANGLIA_MONITOR (ALL)


## Service: HBASE
### MASTER
* HBASE_MASTER (1+)

### SLAVE
* HBASE_REGIONSERVER (1+)
* PHOENIX_QUERY_SERVER (0+)

### CLIENT
* HBASE_CLIENT (1+)


## Service: HDFS
### MASTER
* NAMENODE (1-2)
* SECONDARY_NAMENODE (1)
* HISTORYSERVER

### SLAVE
* DATANODE (1+)
* JOURNALNODE (0+)
* ZKFC (0+)
* NFS_GATEWAY (0+)

### CLIENT
* HDFS_CLIENT (1+)


## Service: HIVE
### MASTER
* HIVE_METASTORE (1)
* HIVE_SERVER (1)
* WEBHCAT_SERVER (1)
* MYSQL_SERVER (0-1)
* POSTGRESQL_SERVER (0-1)

### CLIENT
* HIVE_CLIENT (1+)
* HCAT (1+)


## Service: KAFKA
### MASTER
* KAFKA_BROKER (1+)


## Service: KERBEROS
### MASTER
* KDC_SERVER (0-1)

### CLIENT 
* KERBEROS_CLIENT (ALL)


## Service: KNOX
### MASTER
* KNOX_GATEWAY (1+)


## Service: MAHOUT
### CLIENT
* MAHOUT (0+)


## Service: MAPREDUCE2 (Part of YARN service)
### MASTER
* HISTORYSERVER (1)

### CLIENT
* MAPREDUCE2_CLIENT (0+)


## Service: NAGIOS
* NAGIOS_SERVER


## Service: OOZIE
### MASTER
* OOZIE_SERVER (1)

### CLIENT
* OOZIE_CLIENT


## Service: PIG
### CLIENT
* PIG (0+)


## Service: RANGER
### MASTER 
* RANGER_ADMIN (1-3)
* RANGER_USERSYNC (1)


## Service: RANGER_KMS
### MASTER
* RANGER_KMS_SERVER (1+)


## Service: SLIDER
### CLIENT
* SLIDER (0+)


## Service: SPARK
### MASTER
* SPARK_JOBHISTORYSERVER (1)

### CLIENT
* SPARK_CLIENT (1+)


## Service: SQOOP
### CLIENT
* SQOOP (1+)


## Service: STORM
### MASTER
* NIMBUS (1)
* STORM_REST_API (1)
* STORM_UI_SERVER (1)
* DRPC_SERVER (1)

### SLAVE
* SUPERVISOR (1+)


## Service: TEZ
### CLIENT
* TEZ_CLIENT (1+)


## Service: YARN
### MASTER
* RESOURCEMANAGER (1-2)
* APP_TIMELINE_SERVER (0-1)

### SLAVE
* NODEMANAGER (1+)

### CLIENT
* YARN_CLIENT (1+)


## Service: ZOOKEEPER
### MASTER
* ZOOKEEPER_SERVER (1+)

### CLIENT
* ZOOKEEPER_CLIENT (1+)