#       Hadoop on ec2

*  Type this to download hadoop package
        
        wget http://us.mirrors.quenda.co/apache/hadoop/common/hadoop-2.8.5/hadoop-2.8.5.tar.gz
*   Open jdk Java

        $ sudo apt-get install openjdk-8-jdk
*   Type this to know the path of jdk install

        readlink -f $(which java)



### Create ssh file for easy login (local machine)

*   touch ~/.ssh/config
*   vi ~/.ssh/config
    *   Host namenode
  HostName ec2-18-216-40-160.us-east-2.compute.amazonaws.com
  User ubuntu
  IdentityFile ~/.ssh/MyLab_Machine.pemHost datanode1
  HostName ec2-18-220-65-115.us-east-2.compute.amazonaws.com
  User ubuntu
  IdentityFile ~/.ssh/MyLab_Machine.pem

*   Assuming your private key MyLab_Machine.pem is in .ssh. If it isn't be sure to move or copy it there: cp key_file ~/.ssh/MyLab_Machine.pem

*   Type below command to see your login is easy or not
    
        ssh namenode

*   Copy ssh file to the instance

        scp ~/.ssh/config namenode:~/.ssh

*   Use the below command to generate key for connection of datanode and namenode (do it on namenode)

    *   $ ssh-keygen -f ~/.ssh/id_rsa -t rsa -P ""
    *   $ cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys

*   Add this file in namenode (~/.ssh/config file)

                Host 0.0.0.0
	        User hadoopuser
                IdentityFile ~/.ssh/hadoop_key.pem


