<h1>Startup - IAM and Security </h1>



<h2>Project Description</h2>

Project Brief


Client Background:
You are a Cloud Engineer Consultant, working with StartupCo, a fast-growing tech startup that recently launched their first product - a fitness tracking application.

They've been using AWS for three months, initially setting up their infrastructure quickly to meet launch deadlines.

Now that their product is live, they need to address their cloud security fundamentals.  The company has 10 employees who all currently share the AWS root account credentials to access and manage their cloud resources.

This practice started when they were moving quickly to launch, but now their CTO recognizes the security risks this poses.

Current Setup:

Everyone uses the root account

No separate permissions for different teams

No MFA or password policies

AWS credentials shared via team chat

Current Infrastructure:

EC2 instances running their application

S3 buckets storing user data and application assets

RDS database for user information

CloudWatch for monitoring

Several development and production environments

Team Structure & Access Needs: 

  4 Developers (need EC2 and S3 access)

 2 Operations (need full infrastructure access)

 1 Finance Manager (needs cost management access)

 3 Data Analysts (need read-only access to data resources)

--------- Your Task ---------
1 - Create their Architecture

Create a architecture diagram showcasing their current infrastructure



2 - Secure the Root Account

Enable MFA

Stop using it for daily operations

Store credentials securely



3 - Create IAM Users and Groups

Developer group & users

Operations group & users

Finance group & user

Analyst group & users



4 - Set Up Security Requirements

Enable MFA for all users

Create a strong password policy

Ensure users can only access what they need



5 - Implement These Permissions

Developers:

EC2 management

S3 access for application files

CloudWatch logs viewing

Operations:

Full EC2, CloudWatch access

Systems Manager access

RDS management

Finance:

Cost Explorer

AWS Budgets

Read-only resource access

Analysts:

Read-only S3 access

Read-only database access







<h2>Project Architecture</h2>
<img width="994" height="670" alt="image" src="https://github.com/user-attachments/assets/2d4c8d2c-95f3-467d-97d7-6cac49a41562" />


<h2>Project Explanation</h2>

In this project, I addressed a common challenge for startups: moving from a fast launch setup to a secure, scalable cloud environment. Using my security and AWS expertise, I designed a stronger architecture and implemented best practices to protect StartupCo’s infrastructure.

I began by securing the AWS root account. I enabled MFA, stopped using it for daily operations, and created a new administrator account for ongoing management. Locking down the root account is one of the most critical steps in cloud security- if it’s compromised, the entire environment is at risk. I also emphasized separating the management/billing account from operational accounts, aligning with AWS security best practices.

Next, I created IAM users and groups based on job roles and applied the principle of least privilege. Each team- Developers, Operations, Finance, and Analysts, received only the permissions they needed. This structure provides clearer accountability and reduces the risk of unauthorized access.

I also implemented multi-factor authentication for all users and rolled out a strong password policy with expiration and password reuse prevention. This ensures that access credentials remain secure and harder to compromise.

Together, these changes transformed a shared-root-account setup into a well-structured, secure AWS environment tailored to StartupCo’s needs while laying the groundwork for future growth.

<h2>Implementation Screenshots</h2>


<img width="1359" height="666" alt="image" src="https://github.com/user-attachments/assets/942f10ef-4e3f-4c71-b00a-88aac723cbde" />


<img width="1909" height="890" alt="image" src="https://github.com/user-attachments/assets/15a54fde-91d5-4622-8949-692361510181" />


<img width="1908" height="885" alt="image" src="https://github.com/user-attachments/assets/26b8b68b-d593-43e9-820a-abb672e992e8" />


<img width="1904" height="862" alt="image" src="https://github.com/user-attachments/assets/ba974657-3ded-45f8-a405-c1ea2ff6f3fb" />


<img width="1912" height="885" alt="image" src="https://github.com/user-attachments/assets/a6c604cb-3023-4b5d-97c5-e6d6ebf96d83" />


<img width="1910" height="883" alt="image" src="https://github.com/user-attachments/assets/e0b0b9d3-87ac-4c8e-9bf3-ec3c27fa19a4" />


<img width="1906" height="888" alt="image" src="https://github.com/user-attachments/assets/b18579be-80c6-4b5f-b4f7-a4515fae9ded" />


<img width="1909" height="888" alt="image" src="https://github.com/user-attachments/assets/ca2b7e37-2fb5-4e42-90f0-d359203fe4f7" />


<img width="1899" height="894" alt="image" src="https://github.com/user-attachments/assets/3b7e7424-6f03-402e-9f09-a28e7d39ca03" />


<img width="1899" height="890" alt="image" src="https://github.com/user-attachments/assets/11abf41a-f3f3-400c-85d8-659db22079c5" />


<img width="1905" height="883" alt="image" src="https://github.com/user-attachments/assets/1116e36c-7cb4-4d3c-805f-4100c54739ac" />















