##ANSIBLE INTEGRATION WITH JENKINS
* Create a ansible server
  * create a node and configure with ansible master
  * install ansible 
  * create a one user and make him as a admin for that do bellow steps
  ```
  vi /etc/ssh/sshd_configu
    * change passwdauthentication no to yes
  visudo
    * ansible ALL=(ALL:ALL) NOPASSWD: YES  
  ```
# ON JENKINS MASTER 
  * install the configure over ssh plugin
  * go to system config and add the ansible node with ssh      creadiationl ![preview](/images/ssh-server.PNG)  
* select mvn project and select vcs and select post-build steps in that select copy the ssh and give the remote location ![Preview](/images/post-ssh.PNG)  