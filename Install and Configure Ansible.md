# Install Required Packages

1. Check for which repos are enabled. 
```
yum config-manager add-repo="http://repo.example.com/AppStream" 
yum config-manager add-repo="http://repo.example.com/BaseOS" 
```

Make sure repos are enabled by running: 
```
yum repolist all
```

NOTE: yum config-manager --add-repo should  automatically enable the repo

2. Update packages and Install python on control node: 
yum update -y && yum install -y python3-pip

3. Verify that ansible is installed
```
ansible --version
```

# Create a static host inventory file
Refer to `/etc/ansible/hosts` file for example for inventory file

Default template of inventory file: 
```

```






# Create a configuration file
`cat /path/to/folder/ansible.cfg`



Default template of `ansible.cfg` : 
```
[defaults]
inventory=inventory

[privilege_escalation]
```










# Create and use static inventories to define groups of hosts
`cat /path/to/folder/inventory`


Default template of inventory : 
```
[servers]
server1.example.com
server2.example.com

[webservers]
server3.example.com
server4.example.com

[allservers:children]
servers
webservers
```




# Manage parallelism
