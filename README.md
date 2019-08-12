# Monitoring Plugin: Galera cluster

### Description

This fairly simple monitoring plugin monitors the health of your galera cluster (for either Percona or MariaDB).

### Usage

    -h Prints out this message
    -H Hostname [Default: localhost] MySQL (Fork) Server
    -P port [Default: 3306] Port
    -u username [Default: root] Username to monitor (Needs privilege to execute SHOW STATUS)
    -p password [Default: <none>] Password
    -w warning [Default: 1] Script will throw a warning if the number of failed or unreachable nodes is at least the number specified
    -c critical [Default: 2] Script will throw a critical if the number of failed or unreachable nodes is at least the number specified

### Install 

Copy check_galera_cluster to your plugin folder and create a service/exec in your monitoring engine. 
