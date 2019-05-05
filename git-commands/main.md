##git commands
create a git hub account with user name and passwd and make a note of username and passswd.
we shoud configure the git in local repo for that 
1) create a directory in our local machine and intiate git in this directory
```
git init
```
2) configure that directory with git hub username and password i.e
```
git config --global user.name <user-name>
     ex:  git config --global user.name naigreddy-9 
git config --global user.email <our-email> 
     ex: git config --global user.email <somthing@gmail.com>
```     
4) add local repo to remote repo.
```
git remote add origin(anyname) master <url-of-remote-repo>
```
5) if any error in push or pull (if our local machine is configure more than one remote repo
     we should change some setting for previnting the errors i.e follow steps
```
    a) Go to Win -> Control Panel -> Credential Manager -> Windows Credentials
```
  remove old user name and passwd.
and play with git it will ask username and passwd in papup window.
    b) if any un related histories than we should user
```     
git pull --allow-unrelated-histories	 
```