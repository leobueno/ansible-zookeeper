#Zookeeper
Installs [zookeeper](http://zookeeper.apache.org/)

##Requirements
- zookeeper_hosts - comma separated list of host:port pairs, defaults to 'ansible_fqdn:2181' for a single node

##Optional
- zookeeper_log_level - Log level to be used for zookeeper logs. Defaults to WARN
- zookeeper_wait_for_period - The time in seconds for how long to wait for Zookeeper's port to be available after starting it. Default is 30 seconds.
- run_mode: One of Deploy, Stop, Install, Configure or Start. The default is Deploy which will do Install, Configure, then Start.
- zookeeper_id - Id to be used if one can't or shouldn't be derived from zookeeper_hosts. This will happen if zookeeper_hosts doesn't contain the fqdn but an alias
- zookeeper_heap_opt - Java Heap option for the zookeeper process. Default is to let the JRE decide

##Credits

This role is a fork of https://github.com/hpcloud-mon/ansible-zookeeper and was created because I didn't openjdk or any other dependency installed by the kafka role

##License
Apache

##Author Information
Leonardo Bueno

leonardo.bueno@gmail.com
