# cloudformation-vpc
This cloudformation template creates a complete vpc architecture with 
2-public subnets
2-private subnets
2-database subnets

Along with internet gateway, Nat gateway.

3 NACLs one for each type of subnet.

Public NACL allows allow all traffic from outside world

Private NACL allows only traffic from public subnets

Private DB NACL allows only traffic from private subnets

DNS Hostname, Resolution is also enabled on vpc.

Just upload the template in cloudformtion console and provide following details

1- environment name in parameter as it will be prefixed with all resources.
2- Two AZs to make the subnets multi AZ.
