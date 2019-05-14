## VPC PEERING CONFIGURATION
* Take two Regions 
   * OREGON (region)
     * ceate one vpc
       * 10.0.0.0/16
     * two subnets
       * 10.0.0.0/24
       * 10.1.0.0/24
     * creata a internet gate way and attache with vpc
     * create a routetable and edit the roules i.e
       * 0.0.0.0/0  to igw
   * N-VIRGINIA (Region)
     * ceate one vpc
       * 10.10.0.0/16
     * two subnets
       * 10.10.0.0/24
       * 10.10.1.0/24
* Select VPC Peering 
  * create a peering connections with requred details 
  * we should send request to n-virginia so open the that ip 
  * in routetable.
  * go to the n-virginia and we should accept the request of   oregon.       
     * here we should accept the request from oregon so edit * the roules in the route table 
