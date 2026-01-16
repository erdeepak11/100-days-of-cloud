# Day 3: Create Subnet (AWS)

## What was the task?
Create a subnet named **datacenter-subnet** under the **default VPC** in the **us-east-1** region to understand how AWS divides a VPC into smaller network segments.

---

## Step-by-step approach I followed

1. Logged in to the AWS Management Console.
2. Selected the **us-east-1 (N. Virginia)** region to ensure resources are created in the correct region.
3. Used the AWS search bar to search for **VPC**.
4. Opened the **VPC Dashboard**.
5. Navigated to **Subnets** from the left-hand menu.
6. Clicked on **Create subnet**.
7. Selected the **default VPC**.
8. Entered the subnet name as **datacenter-subnet**.
9. Selected a single **Availability Zone**, as a subnet must belong to one AZ.
10. Reviewed existing subnet CIDR blocks in the default VPC to avoid overlap.
11. Entered a valid, non-overlapping IPv4 CIDR block within the VPC CIDR range.
12. Reviewed the configuration and clicked **Create subnet**.

---

## What I configured
- Subnet Name: datacenter-subnet  
- VPC: Default VPC  
- Region: us-east-1  
- Availability Zone: Single AZ  
- IPv4 CIDR block: Non-overlapping range within the VPC CIDR  

---

## What I learned
- A subnet must always be created inside a VPC.
- Subnet CIDR blocks must fall within the VPC CIDR range.
- CIDR overlap is not allowed, even in default VPCs.
- Each subnet belongs to only one Availability Zone.

---

## Real-life use case
In real-world cloud architectures, subnets are used to separate workloads such as public-facing services and internal systems, improving security, availability, and network organization.
