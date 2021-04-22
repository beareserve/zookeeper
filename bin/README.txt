This directory contain scripts that allow easy access (classpath in particular)
to the ZooKeeper server and command line client.

Files ending in .sh are unix and cygwin compatible

Files ending in .cmd are msdos/windows compatible


main方法启动zk需要指定配置文件：
    Run/Debug Configurations——>Configuration——>Program Arguments里加上：
    C:\Users\run\IdeaProjects\zookeeper\conf\wzoo.cfg

这里配置有4种，windows下的单机、集群配置（w开头的配置文件）；mac下的单机集群配置。另外zoo_sample.cfg是zk的官方出厂配置

我这里用wzoo.cfg启动，就是windows下的单机环境。
wzoo.cfg中就修改了一个配置：
    dataDir=C:\\Users\\run\\IdeaProjects\\zookeeper\\data\\zk
这个配置表示的是zk数据备份快照文件的保存路径，还有集群环境下节点的myid文件路径
