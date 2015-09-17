#ansible node app example
ansible-playbook -i hosts -e "type=test" playbooks/test-provision.yml  -vv

##Requirements
Ansible 2 for ec2 - get ansible from source

Boto3 - pip install boto3

##Tested From
One aws intance with full iam role/policy for provisioning etc

.ssh/config setup to reach mongo boxes
 
##Done
###AWS
99% done - need an ELB

3 Nats and VPC

Routing

3 Web in ASG

3 Mongos with static addresses

###APP
Mongo running and configured on one instance

##Refactoring required/suggested so far
NATs as 3 x ASG with size of 1 and ENI for routing

Separate Volumes for Mongos

Permanent IPs and DNS for Nat for ssh forwarding


#TODO:

##AWS 
ELB

Refactor with more loops to be more concise 

Mongo SG

##APP
Node App

3 Node Mongo Scale Out

