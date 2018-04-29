> #### launch aws simple infrastructure

- create keypair
- create security group,open 22,8080 ports.
- create load balancer
- launch ec2 instances,instances are distributed in different available zones.
- initialize ec2 instances,install jdk
- add ec2 instances to load balancer

> #### usage

- set environment variables

$export AWS_ACCESS_KEY_ID=XXXXXXXXXXXX
$export AWS_SECRET_ACCESS_KEY=XXXXXXXXXXXX

- create local key pair (optional)

$ssh-keygen -t rsa 

- modify config file

modify the file of "vars.yml" according to your needs.

- run playbook

$ansible-playbook -i inventory.ini main.yml 

