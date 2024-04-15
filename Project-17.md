## **Documentation for Project 17**

### Automate Infrastructure With IAC using Terraform Part 2

### Creating Private Subnets using the count function and incrementing the count.index value for the cidr block function of our private subnet by 2 so that our subnets will not overlap thereby causing our application to malfunction

![creating-private-subnets-and-adjusting-count-index-value](./Images/creating-private-subnets-and-adjusting-count-index-value.png)

### Terraform plan showing the private subnets that will be created such that it will not overlap with the public subnet

![terraform-plan-showing-the-private-subnets-that-will-be-created](./Images/terraform-plan-showing-the-private-subnets-that-will-be-created.png)

### Tagging our Subnets appropriately using the tag = merge function

![Subnet-tag-1](./Images/Subnet-tag-1.png)

### Declaring tag variables

![declaring-tag-variables](./Images/declaring-tag-variables.png)

### Declaring tag values

![declaring-tag-values](./Images/declaring-tag-values.png)

### Terraform Plan to show our Tags attached to our subnets respectively

![terraform-plan-to-show-our-tags](./Images/terraform-plan-to-show-our-tags.png)

### Creating Internet Gateway and NAT Gateway with Elastic IP

### Creating Internet Gateway in a separate TF file

![internet-gateway-created-in-a-separate-TF-file](./Images/internet-gateway-created-in-a-separate-TF-file.png)

### Creating NAT Gateway in a separate TF file

![nat-gateway-created-in-a-separate-TF-file](./Images/nat-gateway-created-in-a-separate-TF-file.png)

### Elastic IP created alongside our NAT Gateway in the same TF File

![elastic-ip-created-alongside-our-nat-gateway](./Images/elastic-ip-created-alongside-our-nat-gateway.png)

### Terraform Plan to show updated resources about to be created

![overview-of-our-new-resources-eip-nat-igw](./Images/overview-of-our-new-resources-eip-nat-igw.png)

![Total-number-of-resources-to-be-created](./Images/Total-number-of-resources-to-be-created.png)

### Terraform graph to show dependencies

![terraform-graph-to-show-dependencies](./Images/terraform-graph-to-show-dependencies.png)

### Creating AWS Routes and subnet associations

![aws-routes-about-to-be-created-shown-on-terraform-plan](./Images/aws-routes-about-to-be-created-shown-on-terraform-plan.png)

![terraform-apply-showing-aws-routes-and-associations-being-created](./Images/terraform-apply-showing-aws-routes-and-associations-being-created.png)

### Creating a Certificate for our load Balancers

![creating-certificate](./Images/creating-certificate.png)
![certificate-created-after-terraform-apply](./Images/certificate-created-after-terraform-apply.png)

### Creating Security Groups

![creating-certificate](./Images/aws-security-group-created.png)
![aws-security-group-rule-created](./Images/aws-security-group-rule-created.png)

![security-group-created](./Images/security-group-created.png)

### Creating record in our route53 hosted zone

![creating-A-record-in-our-hosted-zone](./Images/creating-A-record-in-our-hosted-zone.png)

![A-record-created](./Images/A-record-created.png)

### Creating Load Balancers

![creating-load-balancers](./Images/creating-load-balancers.png)
![load-balancers-created.png](./Images/load-balancers-created.png)

### Creating Target Groups

![creating-target-groups](./Images/creating-target-groups.png)

![Target-groups-created](./Images/Target-groups-created.png)

### Creating Load Balancer Listener Rule

![creating-listener-rule](./Images/creating-listener-rule.png)
![listener-rule-created](./Images/listener-rule-created.png)

### Creating Launch Template and Auto scaling Group for Bastion, Nginx, wordpress and tooling

### Bastion

![Creating-Launch-Template-for-bastion-terraform](./Images/creating-Launch-Template-for-bastion-terraform.png)
![terraform-bastion-autoscaling-group-created](./Images/terraform-bastion-autoscaling-group-created.png)

### Nginx

![Creating-Launch-Template-for-bastion-terraform](./Images/terraform-launch-template-nginx-created.png)
![terraform-bastion-autoscaling-group-created](./Images/terraform-autoscaling-group-nginx-created.png)

### wordpress

![terraform-launch-template-wordpress-created](./Images/terraform-launch-template-wordpress-created.png)
![terraform-bastion-autoscaling-group-created](./Images/terraform-autoscaling-group-wordpress-created.png)

### tooling

![terraform-launch-template-tooling-created](./Images/terraform-launch-template-tooling-created.png)
![terraform-autoscaling-group-tooling-created](./Images/terraform-autoscaling-group-tooling-created.png)

### Creating Our EFS and Mounting our Webservers on EFS

### Creating EFS Storage for ours Webservers

![efs-created](./Images/efs-created.png)
![efs-live-on-console](./Images/efs-live-on-console.png)

### Mounting our EFS in the Subnet where our resources resides (webservers) for easy accessibility.

![Mounting-our-efs-in-the-subnet-of-our-rersources](./Images/Mounting-our-efs-in-the-subnet-of-our-rersources.png)

### Creating efs Access point for our webservers to connect to the file storage

![efs-accesspoint-for-our-webservers-created](./Images/efs-accesspoint-for-our-webservers-created.png)

### Creating RDS for our Webservers which involves creating a Subnet Group and an RDS Instance

![DB-subnet-group-created](./Images/DB-subnet-group-created.png)

### RDS Instance Created
![RDS-instance-created](./Images/RDS-instance-created.png)
![RDS-instance-created](./Images/DB-instance-live-on-console.png)
