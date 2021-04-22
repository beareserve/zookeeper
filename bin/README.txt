This directory contain scripts that allow easy access (classpath in particular)
to the ZooKeeper server and command line client.

Files ending in .sh are unix and cygwin compatible

Files ending in .cmd are msdos/windows compatible


main方法启动zk需要指定配置文件：
    Run/Debug Configurations——>Configuration——>Program Arguments里加上：
    C:\Users\run\IdeaProjects\zookeeper\conf\wzoo.cfg

这里配置有4种，windows下的单机、集群配置（w开头的配置文件）；mac下的单机集群配置。另外zoo_sample.cfg是zk的官方出厂配置

我这里用wzoo.cfg启动，就是windows下的单机环境。
