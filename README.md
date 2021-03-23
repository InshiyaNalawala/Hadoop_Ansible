# Hadoop_Ansible
This repository provides the code for configuring Hadoop with Ansible on RHEL nodes. 
Here, we are using rpm files to first install jdk and then hadoop.
Before begining, make sure you copy the rpm files in the /root folder on your Controller node. From there it will be copied to the data nodes and installation will be possible only then. 
All the configuration of important files is done through ansible. 
After successfull configuration, the namenode is formatted and the namenode and datanode services are started. 
You can then run the following command, to check the Configured Capacity in the Cluster,
 # hadoop dfsadmin -report 
