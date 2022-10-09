# Method 1

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
