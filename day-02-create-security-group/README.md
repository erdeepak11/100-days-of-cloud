# Day 2: Create Security Group (AWS)

## What was the task?
Create an AWS Security Group in the default VPC with HTTP and SSH inbound rules in the us-east-1 region.

---

## Step-by-step approach I followed

1. Logged in to the AWS Management Console.
2. Selected the **us-east-1 (N. Virginia)** region to ensure resources are created in the correct region.
3. Used the AWS search bar to search for **EC2**.
4. Opened the EC2 dashboard.
5. From the left-hand menu, navigated to **Security Groups** under the Network & Security section.
6. Clicked on **Create security group**.
7. Entered the security group name as **xfusion-sg**.
8. Added the description: **Security group for Nautilus App Servers**.
9. Selected the **default VPC**.
10. Added an inbound rule for **HTTP** with port **80** and source **0.0.0.0/0**.
11. Added another inbound rule for **SSH** with port **22** and source **0.0.0.0/0**.
12. Reviewed the configuration and clicked **Create security group**.

---

## What I configured
- Security Group Name: xfusion-sg
- Inbound HTTP access on port 80
- Inbound SSH access on port 22
- Both rules allow traffic from anywhere (0.0.0.0/0)

---

## What I learned
- Security Groups act as virtual firewalls for EC2 instances.
- Inbound traffic is blocked by default and must be explicitly allowed.
- Security Groups are stateful, so return traffic is automatically permitted.

---

## Real-life use case
In real-world cloud environments, Security Groups are used to control access to servers by allowing only required ports and sources, helping reduce security risks.
