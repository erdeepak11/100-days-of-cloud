## Day 1 - Creating an EC2 key pair (AWS)

### Task overview
The goal of this task was to create an EC2 key pair in AWS as part of the initial steps toward migrating infrastructure to the cloud. This key pair will be used later to securely access EC2 instances.

### What the Task Was About
An EC2 key pair is required for secure, key-based access to Linux EC2 instances. For this task, the requirement was to create an RSA key pair named `nautilus-kp` in the `us-east-1` region.

### How I Approached the Task
I logged in to the AWS Management Console using the provided credentials, ensured the correct region was selected, and created the key pair through the EC2 service. I also made sure to securely store the private key, as it is available for download only once.

### Script / Configuration Context
This task was completed using the AWS Console. In real-world environments, the same step is often automated using YAML-based infrastructure-as-code tools to ensure consistency across environments.

### Key Learning
- Key pairs are mandatory for accessing EC2 instances
- Key pairs are region-specific
- Private keys must be stored securely since they cannot be retrieved again

### Real-World Use Case
In production cloud environments, teams create and manage key pairs before provisioning servers to control access, prevent password-based logins, and maintain strong security standards.
