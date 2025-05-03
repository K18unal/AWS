# AWS
------------------------------------------------------------------
IAM
What 

This is a diagram representing AWS IAM (Identity and Access Management) user roles and permissions within an AWS environment. It shows a hierarchy starting from the Root User and branching into various IAM Users with specific policies assigned to them.


Why 

This diagram exists to demonstrate:
	•	How AWS access and responsibilities are distributed across different users.
	•	Security best practices in AWS, such as:
	•	Avoiding use of the Root User for everyday tasks.
	•	Creating IAM Users with least-privilege access based on job roles.
	•	Separating permissions (admin, EC2, S3) for better control and auditability.


How 

This structure is achieved through AWS IAM by:
	•	Creating IAM Users under the Root User’s AWS account.
	•	Assigning IAM Policies to each user or group to grant specific permissions:
	•	IAM User 1: Has admin access, likely using AWS’s managed AdministratorAccess policy.
	•	IAM Users 2 & 3: Have a policy allowing them to create EC2 instances and Read/Write
