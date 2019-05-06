##SONARQUBE INSTALLATION AND INTEGRATION WITH JENKINS

* To work sonarqube we have java8.
* Add the bellow content to /etc/apt/sources.list
```
 deb [trusted=yes] http://downloads.sourceforge.net/project/sonar-pkg/deb  binary/
 ```
* install java and sonarqube use bellow commands
```
sudo apt-get update
sudo apt-get install openjdk-8-jdk -y
sudo apt-get install sonar -y 
sudo service sonar start
```
* Login with http://<ipaddress:9000>
  * by default sonarqube use 9000 port
* Login default username and passwd's are admin/admin
* After that we should generate token number and select build launguage.


###  Configuring Jenkins and sonar to perform Code Analysis

* Setup a Jenkins server if already not using.
* Goto plugin-manager of Jenkins to install “SonarQube Plugin”.
* Goto “System-configuration” of Jenkins to provide “SonarQube” server’s     details as below.