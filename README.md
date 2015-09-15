#ansible node app example
ansible-playbook -i hosts -e "type=test" playbooks/test-provision.yml  -vv

##Done
3 Nats and VPC
3 Subnets for Web
3 Sunbets for App

##Refactoring required so far
Resuability: Loops for subnets etc
NATs as ASG with size of 1

#TODO:

##AWS 
Internal Routes to NATs
3 Web Servers in ASG
3 Mongo Servers in ASG with 3 Volumes

##APP
Node App
3 Node Mongo

