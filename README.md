# AWS_VPC_Production_Lab


This example illustrates how to set up a VPC for hosting production servers. To enhance resiliency, servers are deployed across two Availability Zones using an Auto Scaling group and an Application Load Balancer. For added security, the servers are placed in private subnets, receiving traffic through the load balancer. Outbound internet access for the servers is facilitated via a NAT gateway, which is deployed in both Availability Zones to ensure high availability.

![image](https://github.com/user-attachments/assets/93b03a39-118a-4cb0-aa4f-1dc80554a6b5)
