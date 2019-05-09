#INSTALL JENKINS ON REDHAT
* To run jenkins must need openjdk 8 
```
yum install java-1.8.0-openjdk
```
* set java home in /etc/environment
```
JAVA_HOME="/usr/lib/jvm/"
```

1) create a user for jenkins

  ```
  adduser jenkins
  passwd jenkins
  ```
2) make him admin priv and passwd less user
   change bellow settings
  ```
  visudo
  vi /etc/ssh/sshd_config
  service sshd restart
  ```  
3) install jenkins go to official doc
```
https://wiki.jenkins.io/display/JENKINS/Installing+Jenkins+on+Red+Hat+distributions
```  
```
    sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
    sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
    sudo yum install jenkins
```