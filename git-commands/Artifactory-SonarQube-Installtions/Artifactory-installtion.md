#ARTIFACTORY INSTALLATION
1) PRERQUSITES:
   * java8 (openjdk is better)
     * UBUNTU
       ```
       sudo apt-get install openjdk-8-jdk -y
       ```
     * REDHAT(Linux)
       ```
       yum install java-1.8.0-openjdk -y
       ``` 
2) SET JAVA_HOME
   * vi /etc/environment
   ```
   JAVA_HOME="/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.212.b04-0.el7_6.x86_64"

   ```
   * Source The Environment
   ```
   source /etc/environment
   ```       
###INSTALL ON UBUNTU 18.04
* Get the artifactory zip file from bellow location.
```
wget https://bintray.com/jfrog/artifactory/download_file?file_path=jfrog-artifactory-oss-6.5.1.zip -O artifactory.zip
```
* Unzip the file and do bellow tasks.
```
unzip artifactory.zip 
cd artifactory-oss-6.5.1/
cd tomcat/
mkdir logs
cd bin/
sh catalina.sh start
```
3)    