# Day 4 – Enable Versioning for S3 Bucket

## 1. What the task is about
The task focuses on enabling **versioning** for an existing S3 bucket to ensure data protection and recovery in case of accidental deletion or overwrite.  
The bucket used in this task is `devops-s3-11894` in the `us-east-1` region using **:contentReference[oaicite:0]{index=0}**.

---

## 2. How I approached the task
I approached this task from a **data protection perspective** rather than just configuration.  
The goal was to understand how versioning helps in maintaining multiple copies of objects and allows recovery of deleted or overwritten files.

Since this was a concept-driven task in a lab environment, I used the **AWS Management Console** to clearly observe where and how versioning is enabled at the bucket level.

---

## 3. Configuration / Script approach (brief)
Instead of writing long scripts, I verified the bucket configuration and enabled versioning at the **bucket properties level**.  
In a real-world scenario, this can also be done using **infrastructure-as-code (YAML)** to define the bucket and its versioning settings declaratively.

---

## 4. What each action does
- Selecting the correct region ensures the correct bucket is managed.
- Opening the S3 bucket allows access to bucket-level configurations.
- Enabling versioning ensures that every change to an object creates a new version.
- Verification confirms that the bucket now protects objects from permanent deletion.

---

## 5. Key takeaway
- Versioning is a **bucket-level feature** in S3.
- Deleted objects are not immediately lost; a delete marker is created.
- Versioning helps protect critical data from accidental changes.
- Once enabled, versioning cannot be fully disabled, only suspended.

---

## 6. Real-life use case
S3 versioning is widely used for:
- Backup and restore mechanisms
- Protecting logs and audit data
- Application data rollback
- Compliance and data recovery scenarios

Enabling versioning is a small configuration change that provides **strong data safety guarantees** in production environments.
