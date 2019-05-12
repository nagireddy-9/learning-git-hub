## CREATETING A REUSABLE IMAGE IN ANY CLOUD
* VARIBLES
  * user variable
  * environmental varible
* BUILDERS:
  * builders for aws cloud
  * builders for azure cloud
  [NOTE] we can create a reusable imsage for any cloud and any virtual machines(i.e vmware). see in packer doc.
* PROVISIONING:
  * AWS provisoner
  * AZURE provisoner
  * DOCKER provisoner 
  * ANSIBLE provisoner
  * CHEF provisoner
  * OpenStack(private cloud) provisoner ......
* ##WE NEED IAM CREDIANTIOALS IN AWS
## FUNCTIONS & ENVIRONMENTAL VARIABLES
* 
* we can't create more than one builders in a same file.
ex::
```
 "builder":[
 {
 "type":"amazon-ebs"

 },{
 "type": "amazon-ebs"
 },
 {
 "type": "azure-arm"
 }
 ]
```
 * in this we will get error is builder 2: builder with name 'amazon-ebs' already exists but i was't try thard one which was azure account.
  




