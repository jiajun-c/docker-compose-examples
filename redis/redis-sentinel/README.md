# Redis sentinel mode

There are 6 nodes, 3 sentinels, 1 master and 2 slaves

## test the function

After down the master node, the slave1 become the master node

```shell
root@halfstar:/data# redis-cli -p 6353
127.0.0.1:6353> info replication
# Replication
role:master
connected_slaves:1
slave0:ip=127.0.0.1,port=6352,state=online,offset=25215,lag=0
master_failover_state:no-failover
master_replid:183849b7907bdb7cff49fc9439aa859354b88de6
master_replid2:9ff5ad925022c6b99402a73066520ca5ac4bd038
master_repl_offset:25215
second_repl_offset:8167
repl_backlog_active:1
repl_backlog_size:1048576
repl_backlog_first_byte_offset:792
repl_backlog_histlen:24424
```




