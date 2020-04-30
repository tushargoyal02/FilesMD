#   Installing hadoop

*   Move to cd /var/lib/libvirt/images
*   qemu-img create -f qcow2 -b exist.qcow2 new.qcow2

*   vim /etc/rc.local
    *   type "dhclient -v"
    *   give permission chmod +x /etc/rc.local


*   Login to each machine and then type

    *   iptables -F
    *   setenforce 0
    *   systemctl disable firewalld


In all machines
*   Do "hostnamectl set-hostname name"

*   Do the entry of each node in "vi /etc/hosts" files like
    *   192.168.122.10 nn

*   check the jdk and hadoop
    *   rpm -q jdk (use tab)
    *   rpm -q hadoop



* Write the entry as in hdfs-site.xml
    *   < property >
    *   < name > dfs.namenode.name.dir < /name>
    *   < value > /name   < /value >
    *   < /property>

*   In core site.xml< configuration>
    *   < property>
    *   < name>fs.defaultFS< /name>
    *   < value> hdfs:192.168.122.197:10003 < /value> 
    *   < /property>
