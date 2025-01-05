# AWS_VPC_Production_Lab


This example illustrates how to set up a VPC for hosting production servers. To enhance resiliency, servers are deployed across two Availability Zones using an Auto Scaling group and an Application Load Balancer. For added security, the servers are placed in private subnets, receiving traffic through the load balancer. Outbound internet access for the servers is facilitated via a NAT gateway, which is deployed in both Availability Zones to ensure high availability.

![image](https://github.com/user-attachments/assets/93b03a39-118a-4cb0-aa4f-1dc80554a6b5)

Step 1: Create a VPC
![image](https://github.com/user-attachments/assets/3b3359dd-8e93-4cfb-9874-6ea46fb01f21)

![image](https://github.com/user-attachments/assets/5eafe2c1-374f-4642-ade2-a33f2e46f039)

Step 2: Create a ASG

An Auto Scaling Group (ASG) in AWS automatically manages EC2 instances to ensure your application has the right capacity to handle demand. It adjusts instance numbers dynamically based on metrics (e.g., CPU usage), schedules scaling for specific times, and maintains high availability by distributing instances across Availability Zones. ASGs replace unhealthy instances, integrate with load balancers for traffic distribution, and optimize costs by scaling resources as needed.

![image](https://github.com/user-attachments/assets/c7774385-2b39-42b6-b237-ccdc005fce5c)

![image](https://github.com/user-attachments/assets/56d9e808-7465-4dde-aa46-0caf522f505d)

you Will need to make sure that the Ec2 instance is in the same VPC
![image](https://github.com/user-attachments/assets/0b152aab-9e42-46ae-8b02-f7665248a706)


